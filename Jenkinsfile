pipeline {
    agent any 
     
    stages{
        stage("get_code"){
            steps{
                sshPublisher(publishers: [sshPublisherDesc(configName: 'devops-trial', transfers: [sshTransfer(cleanRemote: false, excludes: '', execCommand: '', execTimeout: 120000, flatten: false, makeEmptyDirs: false, noDefaultExcludes: false, patternSeparator: '[, ]+', remoteDirectory: '/var/www/opend', remoteDirectorySDF: false, removePrefix: '', sourceFiles: '**/*.php ')], usePromotionTimestamp: false, useWorkspaceInPromotion: false, verbose: false)])
        }
    }

    }     
}
