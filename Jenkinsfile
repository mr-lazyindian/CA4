pipeline {
    agent any

    stages {
        stage('Git') {
            steps {
                git url: 'https://github.com/mr-lazyindian/CA4.git', branch: 'main'
            }
        }
    stage('Deploy'){
           steps{
               sh 'ansible-playbook EC2.yml'
           }
        }  
    }
}
