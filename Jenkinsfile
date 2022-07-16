pipeline{
    agent {label 'Linux'}
    stages{
        stage("git checkout")
        {
            steps{
                    git url: 'https://github.com/akhilesh-007/jaipur123.git', branch: 'main'
                 }
          }
        stage("create custom image using dockerfile")
        {
            steps{
                sh "docker build -t webserver ."
            }
        }
       
        stage("create docker container use webserver image")
        {
            steps{
                sh "docker run -it --name=mywebserver webserver /bin/bash"
            }   
            }
         stage("verify web server running or not ")
        {
            steps{
                sh "curl localhost"
            }   
            }
    }
}
