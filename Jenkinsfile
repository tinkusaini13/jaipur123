pipeline{
    agent any
    stages{
        stage("git checkout")
        {
            steps{
                    git 'https://github.com/akhilesh-007/jaipur123.git'
                 }
          }
        stage("make directory")
        {
            steps{
                sh "mkdir hello7"
            }
        }
        stage("ls image")
        {
            steps{
                    sh "sudo docker images"
                 }
          } 
    }
}
