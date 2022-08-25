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
        stage('Github Push in Promox2') {
			steps {
                    //sshagent(credentials:['2021@Sgt']){
                    //sh 'ssh sgt@192.168.15.215'
                script {
                    sh 'ls'
                    sh 'pwd'
		    sh 'mkdir Hello_world'
                    //docker.withRegistry('192.168.15.215:8084', 'sgt_promox')
                    //dockerapp.push('latest')
                    }
			}
		}
    }
}

