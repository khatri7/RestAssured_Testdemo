pipeline {
    agent any
    
    tools{
        maven "MAVEN_HOME"
    }
    stages {
stage('testing pipeline'){
          steps{
      echo 'test1'
                }
}
    stage('Build'){
          steps{
      echo 'Building'
                }
        }
        stage('Test'){
          steps{
      bat 'mvn test'
              
           publishHTML([allowMissing: false, alwaysLinkToLastBuild: false, keepAll: true, reportDir: 'C:\\Users\\jerjose\\Documents\\Reports', reportFiles: 'index.html', reportName: 'HTML Report', reportTitles: ''])
                }
        }
        stage('Deploy'){
          steps{
      echo 'Deploying'
                }
        }
}
}
