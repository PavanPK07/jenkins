pipeline{
    agent{
        node{
            label 'agent-1'
        }
    }
    environment{
        name = "Pavan"
    }

        stages{
            stage('Hello'){
                steps{
                    echo "hello world from GIT SCM"
                    echo "git trigger"
                    echo "$env.name"
                }
            }
        }

        post{

            always{
                echo "I weill always print this "
            }
        }
}