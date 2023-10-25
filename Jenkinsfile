node {
    stage('print name') {
        print "${env.BRANCH_NAME}"
    }
    stage('Clone') {
        git branch: 'env.BRANCH_NAME', url: 'https://github.com/timtest1562/jenkins-helloworld.git'
    }
    stage('Build') {
        sh '''javac Main.java'''
    }
    stage('Run') {
        sh '''java Main'''
    }
}

