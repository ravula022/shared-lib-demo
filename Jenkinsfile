properties([
  buildDiscarder(logRotator(artifactDaysToKeepStr: '30',
        artifactNumToKeepStr: '',
        daysToKeepStr: '90',
        numToKeepStr: '30')),
  disableConcurrentBuilds(),
])

String RepoBase = 'https://github.com/ravula022'
String RepoAccess = 'ravula022-githubid'


library identifier: 'shared-lib-demo@master', retriever: modernSCM([$class: 'GitSCMSource',
  remote: RepoBase + '/shared-lib-demo.git',
  credentialsId: RepoAccess])

library identifier: 'sharedlibs@master',retriever: modernSCM([$class: 'GitSCMSource',
  remote: RepoBase + '/sharedlibs.git',
  credentialsId: RepoAccess])
