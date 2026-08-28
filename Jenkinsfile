pipeline{
    agent any;
    stages{
        stage("Code"){
            steps{
                git url: "https://github.com/Hero9876s/pachnanda-and-associates.git", branch: "master"
            }
        }
        stage("Build"){
            steps{
                bat "docker build -t pachnanda-and-associates ."
            }
        }
        stage("Test"){
            steps{
                 bat "docker image inspect pachnanda-and-associates"
            }
        }
        stage("Push to Docker Hub") {
    steps {
        withCredentials([usernamePassword(
            credentialsId: "DockerHubCreds",
            passwordVariable: "dockerHubPass",
            usernameVariable: "dockerHubUser"
        )]) {
            bat "docker login -u ${env.dockerHubUser} -p ${env.dockerHubPass}"
            bat "docker image tag pachnanda-and-associates ${env.dockerHubUser}/pachnanda-and-associates:latest"
            bat "docker push ${env.dockerHubUser}/pachnanda-and-associates:latest"
        }
    }
}
        stage("Deploy"){
            steps{
                bat "docker rm -f pachnanda-app 2>NUL || exit /b 0"
                bat "docker run -d --name pachnanda-app -p 3000:3000 pachnanda-and-associates"
            }
        }
        
    }
}
