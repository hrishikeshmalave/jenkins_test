pipeline{
    agent any
    stages{
        stage('create'){
            steps{
                echo 'Creating Directory.'
                sh 'mkdir -p /tmp/testdir'
            }
        }
        stage('change directory'){
            steps{
                echo 'Changing Directory.'
                sh 'cd /tmp/testdir'
            }
        }
        stage('create and edit'){
            steps{
                echo 'Creating and editing files...'
                sh 'echo "Hello World" > /tmp/testdir/hello1.txt'
            }
        }
        stage('view'){
            steps{
                echo 'Viewing files...'
                sh 'cat /tmp/testdir/hello1.txt'
            }
        }
    }
}
