pipeline {


     environment {'aws'}

   agent  any

    stages {
        

        stage('Plan') {
            steps {
                sh 'echo $AWS_ACCESS_KEY_ID'
                sh 'pwd'
                sh 'cd course_project ; terraform init -input=false'
                sh "cd course_project ;terraform plan -input=false -out tfplan "
            }
        }
        stage('Apply') {
            steps {
                sh "cd course_project ; terraform apply -input=false tfplan"
            }
        }
    }

  }