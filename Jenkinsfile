pipeline{
    agent any
    stages{
        stage('Compile'){
            steps{
                echo 'Compiled Successfully!!!!';
            }
        }
    stage('JUnit'){
            steps{
                echo 'JUnit Passed Successfully!!!!';
            }
        }
    stage('Deploy'){
            steps{
                echo 'Pass!!!!';
            }
        }
    }
    post{
        always{
            echo "This will always run"
        }
        success{
            echo "This will run if it runs successfull"
        }
        failure{
            echo "This will run if failed"
        }
        unstable{
            echo "This will run only if the run was unstable"
        }
        changed{
            echo "This will run if the state of pipeline has changed"
            echo "For eg, if pipeline was previously failing but it is now successful"
        }
    }
}

