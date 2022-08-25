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
		    sh 'mkdir Hello_world'
		    sh 'pwd'
                    //dockerapp.push('latest')
                    }
			}
		}
    }
}

