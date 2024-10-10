pipeline {
    agent any 
    stages {
        stage("maven build"){
            when {
                branch 'develop'
            }
            steps {
                echo "maven build"
            }
        }
         stage("sonar analysis"){
            when {
                branch 'develop'
            }
             steps {
                echo "sonar analysis"
             }
        }
         stages("vulnarability scaninng"){
            when {
                branch 'develop'
            }
             steps {
                echo "vulnarability scanning"
             }
        }
         stages("dev deploy") {
            when {
                branch 'develop'
            }
             steps {
                echo "dev deploy"
             }
        }
         stages("test deploy") {
            when {
                branch 'test'
            }
             steps {
                echo "test deploy"
            }
        }
        stages("prod deploy"){
            when{
                branch 'main'
            }
             steps {
                echo "prod deploy"
            }
        }
         
    }
}
