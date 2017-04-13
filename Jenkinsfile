#!/usr/bin/env groovy
//Leave the above line alone.  It identifies this as a groovy script.

//Modify the below parameters to match the values for this particular repo

def utfPath = "source\\write.lvproj"
def vipbPath = "Build Test - 2014.vipb"
def lvVersion = "14.0"
def repoName = "SE_Test"

//Leave the below line alone.  It pulls in the pipeline definition from the DCAF buildsystem repo so we don't duplicate code in every repo 
//dcafPipeline(utfPath,vipbPath,lvVersion,repoName)
node{
  echo 'Sending emails out if build failed'
  currentBuild.result = 'FAILURE'
  step([$class: 'Mailer', notifyEveryUnstableBuild: true, recipients: emailextrecipients([[$class: 'CulpritsRecipientProvider'], [$class: 'RequesterRecipientProvider']])])

}
