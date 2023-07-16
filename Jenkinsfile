pipeline { 
agent any 
    stages { 
        stage ('Build') { 
            steps {
                //sudo yum install wget
                echo 'Building dummy project....'
            }
        }
        stage ('Test') { 
            steps {
                echo 'adding dummy tests...'
            }
        }
        stage ('QA') {
              steps {
                  echo 'its QA env'
              } 
        }
        stage ('Deploy') {
               steps {
                   echo 'Deployin on QA environment'
                   emailext body: 'check please ', subject: 'build failed', to: 'kiransp77@gmail.com'
               } 
        }
        
 
    }           
 }
