pipeline {
    agent any
    stages {
   stage('build a source code') {
            when {
                not { branch 'origin/master' }
            }
            steps {
                echo 'building a source code'
            }
        }
        stage('build and deploy artifact') {
            when {
                branch 'origin/master'
            }
            steps {
                echo 'building and deploying artifact'
            }
        }
    }
}
