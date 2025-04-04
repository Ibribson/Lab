pipeline {
    agent any
    stages {
        stage('Cloner le projet') {
            steps {
                echo 'Clonage du dépôt...'
                git 'https://github.com/Ibribson/Lab'
            }
        }
        stage('Construire') {
            steps {
                echo 'Compilation en cours...'
                sh 'mvn clean install'  // Modifier selon la technologie
            }
        }
        stage('Déploiement') {
            steps {
                echo 'Déploiement terminé avec succès !'
            }
        }
    }
}
