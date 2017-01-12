#!/usr/bin/env groovy
import groovy.json.JsonOutput
//Leave the above lines alone.  They identify this as a groovy script and handle necessary immports

//Modify the below parameters to match the values for this particular repo

def utfPath = "source\\write.lvproj"
def vipbPath = "Build Test.vipb"
def lvVersion = "14.0"
def repoName = "SE_Test"


//Leave the below line alone.  It pulls in the pipeline definition from the DCAF buildsystem repo so we don't duplicate code in every repo 
dcafPipeline(utfPath,vipbPath,lvVersion,repoName)
