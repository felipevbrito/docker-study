pipeline {
	agent any

	stages {
		stage('Inicial') {
			steps {
				echo 'Teste de pipeline'
			}
		}
        stage('Get Source') {
			steps {
				git url:  'https://github.com/felipevbrito/docker-study.git', branch: 'main'
			}
        stage('Docker Push Image') {
			steps {
                script {
                    docker.withRegistry('192.168.15.215:8084', 'sgt_promox')
                    dockerapp.push('latest')
                }
			}
		}
	}
}

