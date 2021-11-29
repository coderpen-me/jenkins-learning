pipeline {
    agent any
    stages {
        stage('init') {
            steps {
                sh 'echo "Init Job"'
            }
        }
        stage('trigger_job_1') {
            steps {
                sh 'curl --user admin:admin 'http://localhost:8080/job/job1/build?token=job1''
            }
        }
        stage('trigger_job_2') {
            steps {
                sh 'curl --user admin:admin 'http://localhost:8080/job/Job2/build?token=job2''
            }
        }
    }
}