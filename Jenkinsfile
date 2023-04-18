pipeline {
    agent any
    stages {
        stage('Create Jira Ticket') {
            steps {
                script {
                    def jiraServer = "https://m2iformation.atlassian.net/rest/api/2/issue/"
                    def jiraUser = "maher.hammouda.ing@gmail.com"
                    def jiraPassword = "ATATT3xFfGF0Jzfh5-432ovIpXbVrJwfgeL6afLoePB7CrR0hWl5TyNvWraRpqG6dMiCnTpe0hzFcWQOGzZ5DDPu-7srEY7FVePxgHgZ_nGqxESVC89AX0ie4HdIwdbh_aytJdm9HO4wfyQCnDMYcuAT8XjrxVgdHqM57JNkQxU6StgXTrCrS9s=011288D8"
                    def issueSummary = "My Ticket"
                    def issueDescription = "By Maher"
                    def issueType = "Bug" // Replace with the issue type you want to create
                    
                    def jira = jiraNewServer(serverUrl: jiraServer, username: jiraUser, password: jiraPassword)
                    def issue = jiraNewIssue(serverId: jira.id, fields: [
                        summary: issueSummary,
                        description: issueDescription,
                        issuetype: [
                            name: issueType
                        ]
                    ])
                    
                    echo "Jira ticket created with key: ${issue.key}"
                }
            }
        }
    }
}
