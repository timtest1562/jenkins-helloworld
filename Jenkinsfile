node {
    print "${env.BRANCH_NAME}"
    stage('Clone') {
        git 'https://github.com/timtest1562/jenkins-helloworld.git'
    }
    stage('Build') {
        sh '''javac Main.java'''
    }
    stage('Run') {
        sh '''java Main'''
    }
}
