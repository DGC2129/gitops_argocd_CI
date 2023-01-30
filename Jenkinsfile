pipeline{

    agent any

    environment{

        DOCKERHUB_USERNAME = "gopidevopskanna"
        APP_NAME = "gitops=argo-app"
        IMAGE_TAG = "${BUILD_NUMBER}"
        IMAGE_NAME = "${DOCKERHUB_USERNAME}" + "/" + "${APP_NAME}"
        REGISTRY_CREDS = "Docker Credentials"
    }

    stages{
        stage("Clean the workspace"){
            steps{
                script{

                    cleanWs()
                }
            }
        }
    }
}
