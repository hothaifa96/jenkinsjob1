pipeline {
    agent any 

    environment{
        NAME = 'hothaifa zoubi'
        cloneRepo = ''
        DHCU=''
        DHCP=''
        
    }

    stages {
        stage('fetching'){
            steps {
                sh 'echo $NAME '

                timeout(time: 3 ,unit: 'seconds') {
                     sh 'sleep 5'
                }
            }
        }  
        stage('build'){
            steps{
                retry(3){
                    sh '''
                        echo "finished"
                    '''
                }
                
            }
        }  
        
    }
}