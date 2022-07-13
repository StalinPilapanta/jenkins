pipeline{
    agent any
    stages{
        stage('Build Main'){
           //when{
           //    branch 'main'
           //}
           //steps{
           //    echo 'Build Main'
           //}
           when{
                buildingTag()
            }
            steps{
                echo 'Hello world tag'
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
    }
}