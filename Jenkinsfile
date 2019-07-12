pipeline {
    agent any
    tools { 
        maven 'maven_3_6' 
        jdk 'java_1_8' 
    }
    stages {
        stage ('Compile Stage') {

            steps {
              
                    sh 'mvn clean compile'
               
            }
        }

        stage ('Testing Stage') {

            steps {
                
                    sh 'mvn test'
              
            }
        }

        stage ('Package Stage') {

            steps {
                
                    sh 'mvn clean package'
              
            }
        }
      
    }
}
