node('docker') {

    stage 'Checkout'
        scm Checkout
    stage 'Build & UnitTest'
        sh 'docker build -t accountownerapp:latest -f Dockerfile .'
        sh 'docker build -t accountownerapp:test -f Dockerfile.Integration .'
    
    stage 'Integration Test'

}