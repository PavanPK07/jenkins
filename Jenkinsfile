pipeline{
    agent{
        node{
            label 'agent-1'
        }
    }
    environment{
        name = "Pavan"
    }

    options{
        timeout( time: 1, unit: "HOURS")
        disableConcurrentBuilds()
    }

    parameters{
        text(name: Biography, defaultValue: "uspoken chemistry")
    }

        stages{
            stage('Hello'){
                steps{
                    echo "hello world from GIT SCM"
                    echo "git trigger"
                    echo "$env.name"
                    echo "Biography: ${params.BIOGRAPHY}"
                }
            }
        }

        post{

            always{
                echo "I weill always print this "
            }
        }
}