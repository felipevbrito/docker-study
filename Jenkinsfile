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
        }
        stage('Github Push in Promox') {
			steps {
                script {
                    sh 'ssh sgt@192.168.15.215', 'sgt_promox'
                    //docker.withRegistry('192.168.15.215:8084', 'sgt_promox')
                    //dockerapp.push('latest')
                }
			}
		}
    }
}
