#!/usr/bin/env groovy

pipeline {
  environment {
    MSBUILD = "msbuild"
    BuildType = 'Release'
  }
  stages {
    stage('Build') {
      steps {
        bat "\"${MSBUILD}\" AppNew.csproj /p:BuildType=${env.BuildType}"
      }
    }
  }
}