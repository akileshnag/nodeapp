#!/usr/bin/env groovy

## Groovy Scripting for Jenkins Pipeline

pipeline {



    agent {

        docker {

            image 'node'

            args '-u root'

        }

    }



    stages {

        stage('Build') {

            steps {

                echo 'Building...'

                sh 'npm install'

            }

        }

        stage('Test') {

            steps {

                echo 'Testing...'

                sh 'npm test'

            }

        }

    }

}
