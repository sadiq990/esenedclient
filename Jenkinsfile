pipeline{
    agent any
    stages{
        stage("build"){
            steps{
                script {
                    echo "building the application "
                    
                }
            }
           
        }
        stage("deploy"){
            steps{
                script {
                    echo "deploying the application ..."
                    // withCredentials([usernamePassword(credentialsId: 'docker_hub_password' , passwordVariable: 'PASS' usernameVariable: 'USER' )]){
                    //    sh 'docker build -t sadiq990/nurlanapplication .'
                    //    sh "echo $PASS | docker login -u $USER --passsword-stdin" 
                    //    sh 'docker push'
                    }
                }
            }
           
        }
    }
} 
