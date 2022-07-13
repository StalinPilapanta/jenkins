pipeline{
    agent any
    stages{
        stage('Build Main'){
           when{
               branch 'main'
           }
           steps{
               echo 'Build Main'
           }
        }
        stage('Build Dev'){
            when{
                branch 'dev'
            }
            steps{
                echo 'Build Dev'
            }
        }
        stage('Build Tags'){
            when{
               // buildingTag()
               tag "1.0"
            }
            steps{
                echo 'Hello world tag'
            }
        }

    }
}