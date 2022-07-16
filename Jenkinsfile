pipeline{
    agent any
    stages{
        stage("git checkout")
        {
            steps{
                    git url: 'https://github.com/akhilesh-007/jaipur123.git', branch: 'new-branch'
                 }
          }
        stage("make directory")
        {
            steps{
                sh "mkdir hello3"
            }
        }
        stage("create image")
        {
            steps{
                    sh "docker run -itd --name ng nginx /bin/bash"
                 }
          } 
    }
}
