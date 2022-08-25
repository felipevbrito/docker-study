pipeline {
	agent any

	stages {
		stage('Inicio') {
			steps {
				echo 'Teste de pipeline'
			}
		}
        stage('Puxando do Git') {
			steps {
				git url:  'https://github.com/felipevbrito/docker-study.git', 
				branch: 'main'
			}
        }
        stage('Msg no terminal') {
			steps {
                script {
                    sh 'ls'
                    sh 'pwd'
		    sh 'mkdir Hello_world'
		    sh 'pwd'
                    //docker.withRegistry('192.168.15.215:8084', 'sgt_promox')
                    //dockerapp.push('latest')
                    }
			}
		}
    }
}

