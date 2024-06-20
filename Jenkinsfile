/*This is the pipeline of SF138A_RackPosnTrakgCtrl Dashboard*/
pipeline {
    agent any

    stages {
        stage('Design Phase') {
            parallel{
                stage('Design'){
                    stages{
                        stage('Design Preparation') {
                            steps {
                                echo 'Design Preparation'
                            }
                        }
                        stage('Design Building') {
                            steps {
                                echo 'Design Building'
                            }
                        }
                        stage('Design Review Request') {
                            steps {
                                echo 'Design Review Requestp'
                            }
                        }
                        stage('Design RTC Delivery') {
                            steps {
                                echo 'Design RTC Delivery'
                            }
                        }
                    }
                }
            }
        }
        stage("MIL and Implementation Phase") {
            parallel {
                stage("MIL") {
                    stages{
                        stage('MIL Preparation') {
                            steps {
                                echo 'MIL Preparation'
                            }
                        }
                        stage('MIL Building') {
                            steps {
                                echo 'MIL Building'
                            }
                        }
                        stage('MIL Review Request') {
                            steps {
                                echo 'MIL Review Requestp'
                            }
                        }
                        stage('MIL RTC Delivery') {
                            steps {
                                echo 'MIL RTC Delivery'
                            }
                        }
                    }
                }
                stage("Impl") {
                    stages{
                        stage('Impl Preparation') {
                            steps {
                                echo 'Impl Preparation'
                            }
                        }
                        stage('Impl Building') {
                            steps {
                                echo 'Building'
                            }
                        }
                        stage('Impl Review Request') {
                            steps {
                                echo 'Impl Review Requestp'
                            }
                        }
                        stage('Impl RTC Delivery') {
                            steps {
                                echo 'Impl RTC Delivery'
                            }
                        }
                    }
                }
            }
        }
        stage('SIL Phase') {
            parallel{
                stage('SIL'){
                    stages{
                        stage('SIL Preparation') {
                            steps {
                                echo 'SIL Preparation'
                            }
                        }
                        stage('SIL Building') {
                            steps {
                                echo 'SIL Building'
                            }
                        }
                        stage('SIL Review Request') {
                            steps {
                                echo 'SIL Review Requestp'
                            }
                        }
                        stage('SIL RTC Delivery') {
                            steps {
                                echo 'RTC Delivery'
                            }
                        }
                    }
                }
            }
        }
    }
    post {
        always {
            echo 'This will always run'
        }
        success {
            echo 'This will run only if successful'
        }
        failure {
            echo 'This will run only if failed'
        }
        unstable {
            echo 'This will run only if the run was marked as unstable'
        }
        changed {
            echo 'This will run only if the state of the Pipeline has changed'
            echo 'For example, if the Pipeline was previously failing but is now successful'
        }
    }
}

