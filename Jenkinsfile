#!/usr/bin/env groovy

pipeline {
  environment {
    MSBUILD = "C:\Program Files (x86)\MSBuild\14.0\Bin"
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