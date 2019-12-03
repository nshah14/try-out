pipeline {
    agent { label 'kube' }

   stages {
      stage('Git Checkout ') {
         steps {
            // git clone https://mtlstash.gv.grassvalley.com/scm/lt/devops.git
          sh '''
             git clone --single-branch --branch cherrypy-with-logging https://10.162.1.15/scm/mtlstash/lt/portmanagerws.git
          '''
         }
      }
      stage('Docker Build Checkout ') {
         steps {
            echo 'Docker build '

         }
      }
      stage('Docker tag ') {
         steps {
            echo 'Docker tag the image  World'
         }
      }
      stage('Docker push in local repository ') {
         steps {
            echo 'Docker push into local repo'
         }
      }
      stage('Run kubectl commands for mariadb ') {
         steps {
            echo 'Deploy image in to dev environment'
         }
      }
      stage('Run sql scripts for mariadb ') {
         steps {
            echo 'run sql script on respective mariadb'
         }
      }
      stage('Run kubectl command for LTM ') {
         steps {
            echo 'Deploy image in to dev environment'
         }
      }
   }
}
