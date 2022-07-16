pipeline{
    agent {label 'Linux'}
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
                sh "m"
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
         stage("docker create")
        {
            steps{
                sh "docker run -itd ubuntu"
            }   
            }
    }
}
