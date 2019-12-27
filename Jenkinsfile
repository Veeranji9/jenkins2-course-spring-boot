pipeline {
  agent any
  stages {
    stage('Source') { 
      steps {
			// Check out Step
	      checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/g0t4/jenkins2-course-spring-boot.git']]])
      }
    }
    stage('Compile') { 
      tools {
        // Specify Tool Name from your global tool configuration
		jdk 'jdk1.8.0'
        maven 'maven-3.6.3'
      }
      steps {
			// Some Step
      }
    }
  }
}
