pipeline {
    agent any
    stages {
   stage('build a source code') {
            when {
                not { branch 'master' }
            }
            steps {
                echo 'building a source code'
            }
        }
        stage('build and deploy artifact') {
            when {
                branch 'master'
            }
            steps {
                echo 'building and deploying artifact4'
            }
        }
    }
    post { 
        always { 
            githubnotify  status: "OK"
        }
    }
}
