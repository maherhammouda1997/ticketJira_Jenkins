pipeline {
    agent any
    stages {
        stage('Create Jira Ticket') {
            steps {
                sh 'curl -D- -u maher.hammouda.ing@gmail.com:ATATT3xFfGF0Jzfh5-432ovIpXbVrJwfgeL6afLoePB7CrR0hWl5TyNvWraRpqG6dMiCnTpe0hzFcWQOGzZ5DDPu-7srEY7FVePxgHgZ_nGqxESVC89AX0ie4HdIwdbh_aytJdm9HO4wfyQCnDMYcuAT8XjrxVgdHqM57JNkQxU6StgXTrCrS9s=011288D8 -XPOST --data \'{"fields":{"project":{"key":"TIC"}, "summary":"Create a JIRA Ticket.", "description": "By Maher", "issuetype":{"name":"Bug"}}}\' -H "Content-Type: application/json" https://m2iformation.atlassian.net/rest/api/2/issue/TIC-1'
            }
        }
    }
}