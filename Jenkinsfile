pipeline {
    agent any 
     tools {nodejs "recent node"}
    stages {
        stage('Clonar') { 
            steps {
                git branch: 'main', url: 'https://github.com/anaeuz/exercicio-final-cypress.git' 
            }
        }
        stage('Instalar') { 
            steps {
                sh 'npm install' 
            }
        }
        stage('Executar') { 
            steps {
                sh 'npx cypress run' 
            }
        }
    }
}