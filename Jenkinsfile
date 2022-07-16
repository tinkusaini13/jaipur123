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
                sh "mkdir hi"
            }
        }
        stage("cd hello")
        {
            steps{
                    sh "cd hi"
                 }
          } 
        stage("docker container")
        {
            steps{
                sh "docker images"
            }   
            }
    }
}
