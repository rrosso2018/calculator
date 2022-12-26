pipeline {
    agent any
    stages {
        stage("Checkout") {
            steps {
                git url: 'https://github.com/rrosso2018/calculator.git',branch:'main'
                echo 'Checkout'
            }
        }
        stage("Compile") {
            steps {
                sh "./gradlew compileJava"
                echo "Compile"
            }
        }
        stage("Unit test") {
            steps {
                sh "./gradlew test"
                echo "Test"
        }
}
    }
}
