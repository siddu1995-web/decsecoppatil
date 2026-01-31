pipeline{
    agent any
    stages{
        stage("TEST"){
            when{
                changeset "praveen.yaml"
            }
            steps{
                sh("sudo yum install python3-pip* -y")
            }
        }
        stage("DEV"){
            when{
                changeset "praveen.yaml"
            }
            steps{
                sh ("pip --version")
            }
        }
        stage("DEV1"){
            when{
                changeset "praveen.yaml"
            }
            steps{
                sh("sudo pip3 install ansible")
            }
        }
        stage("PRD"){
            when{
                changeset "praveen.yaml"
            }
            steps{
                sh("ansible --version")
            }
        }
        stage("POSTPRID"){
            when{
                changeset "praveen.yaml"
            }
            steps{
                sh("ansible localhost -m shell -a 'uptime'")
                sh ("cp $WORKSPACE/praveen.yaml /tmp")
                sh("ansible-playbook /tmp/praveen.yaml")
            }
        }
        
            
    }
    post{
        always{
            echo "Needd to check build success r not"
        }
        failure{
            echo "Build is failed"
        }
        success{
            echo "Build is success"
        }
    }
}
