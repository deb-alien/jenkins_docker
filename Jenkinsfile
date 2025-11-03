pipeline {
      agent {
            node {
                  label 'docker-agent-python'
            }
      }

      triggers {
            pollSCM('*/5 * * * *')
      }

      stages {
            stage('Build') {
                  steps {
                        echo 'Building...'
                        sh '''
                        echo "Doing build stuff.."
                        '''
                  }
            }

            stage('Test') {
                  steps {
                        echo 'Testing...'
                        sh '''
                        echo "Doing test stuff.."
                        '''
                  }
            }

            stage('Deliver') {
                  steps {
                        echo 'Deploying...'
                        sh '''
                        echo "Doing deploy stuff.."
                        '''
                  }
            }
      }
}
