pipeline {
    agent any
    stages {
        stage('Create Jira Ticket') {
            steps {
                script {
                    def jiraServer = "https://m2iformation.atlassian.net/rest/api/2/issue/"
                    def jiraUser = "Maher Hammouda"
                    def jiraPassword = "79911997mM."
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
