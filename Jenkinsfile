pipeline{
    agent{
         node {
        label 'agent-1'
    }
    }
    environment { 
        greeting = "good morning baby"
    }
    stages{
         stage("hello")
         {
        steps{
             
            echo "hello world divya"
            }
         }
        stage("hi")
         {
        steps{
             
            echo "hi divya"
        }
    }
    stage("good morning")
    {
        steps{
             
            sh """
            echo "good morning divya"
            echo $env
            """
        }
    }
}
 post { 
        always { 
            echo 'I will always say Hello again!'
        }
        success { 
            echo 'I will always say success!'
        }
                failure { 
            echo 'I will always say success!'
        }
    }
    }