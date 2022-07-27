pipeline {
    agent any 
    // build section
    stages {
        stage("build image") {
            steps {
                script {
                    echo "building the docker image"
                    withCredentials([usernamePassword(credentialsId: 'docker_hub_password' , passwordVariable: 'PASS' , usernameVariable: 'USER' )]) {
                        sh 'docker build -t sadiq990/nurlanapp .'
                        sh " echo $PASS  docker login -u $USER --pasword-stdin"
                        sh 'docker push sadiq990/frontendapp'
                    }
                }
            }
        }
        //deploy section 
        stage("build") {
            steps {
                script {
                    echo "deploying the application"
                }
            }
        }
    }
