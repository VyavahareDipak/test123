pipeline{
  agent any
  environment{
    PYTHON_PATH = 'C:\\Users\\HP\\AppData\\Local\\Programs\\Python\\Python310;C:\\Users\\HP\\AppData\\Local\\Programs\\Python\\Python310\\Scripts'
  }
  stage{
    stage('checkout'){
      steps{
        checkout scm
      }
    }
  }
  stage('build'){
    steps{
      bat '''
      set PATH=%PYTHON-PATH%;%PATH%
      pip install -r requirment.txt
      '''
    }
  }
  stage('Sonarqube-Analysis'){
    environment{
      SONAR-TOKEN = credentials('sonar-token')
    }
    step{
      bat '''
          set 
    }
  }
    
}
