pipeline {
	agent any
    stages {
        stage('build') {
            steps {
                sh 'git config user.name "Jenkins"'
            	sh 'git checkout main'
                sh 'echo "hey" > test.scala'
                sh 'git add test.scala'
                sh 'git commit -am "test: adding a new file"'
                sh 'git push'
            }
        }
    }
}
