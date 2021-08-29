pipeline {
    agent any
    parameters {
        string(
            name: 'FirstName',
            defaultValue: 'World',
            description: 'You can specify your name for personalizing the greeting. If you don\'t specify anything, it will greet you with a "Hello, World!',
            trim: true
        )
    }
    stages {
        stage('Meet') {
            steps {
                echo "Hello, ${params.FirstName}!"
            }
        }
        stage('Leave') {
            steps {
                echo "Bye, ${params.FirstName}!"
            }
        }
        stage('Cleanup') {
            steps {
                echo "This is a dummy clean-up stage."
            }
        }
        stage('Goodbye') {
            steps {
                echo "I am done."
            }
        }
    }
}
