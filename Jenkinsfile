pipeline {
         agent any
         stages {
                 stage('Initialize'){
                 def dockerHome = tool 'Docker1'
                 env.PATH = "${dockerHome}/bin:${env.PATH}"
                  }
                 stage('Stage One') {
                 steps {
                     echo 'Hi, welcome to SCM pipeline demo...'
                 }
                 }
                 stage('Stage Two') {
                 steps {
                    //echo('Sample testing of Stage 2')
                    echo('Creating docker image')
                    sh ' docker build -t testapp:1.0 . '
                 }
                 }
                 stage('Stage Three') {
                
                 steps {
                       echo 'Thanks for using Jenkins Pipeline'
                 }
                 }
              }
}
