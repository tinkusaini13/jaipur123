pipeline{
    agent any
    stages{
        stage("git checkout")
        {
            steps{
                    git url: 'https://github.com/akhilesh-007/jaipur123.git', branch: 'main'
                 }
          }
        stage("make directory")
        {
            steps{
                sh "mkdir hello2"
            }
        }
        stage("ls image")
        {
            steps{
                    sh "docker run -itd nginx"
                 }
          } 
    }
}
