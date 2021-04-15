pipeline {
    environment {
    addresbook = "jarrayaahmed99/addresbook"
    registryCredential = 'dockerpassword'
    addressbook=''
    }
agent any
    stages{
   stage('pwd')
    {
      steps {
        sh'pwd'
            }   
    }
        
    
stage('Checkout Source')
    {
      steps {
        git url:'https://github.com/JarrayaAhmed99/dockerizing-nodejs.git', branch:'master'
            }
     }
        
         stage('building addressbook image')
    {
      steps {
          script
          {
        addressbook= docker.build(registry1 , "-f ${env.WORKSPACE}/Dockerfile.development .")
          } 
          }   
    }
        
        
        
        
        
        
          }




}
