pipeline {
    agent any
    stages {
        stage ('Get update'){
            sh 'sudo apt-get install apache2 -y'
        }
        stage ('Get started'){
            sh 'sudo sytemctl start apache2'
        }
        stage ('remove exiting html files'){
            sh 'sudo rm -f /var/www/html/*'
        }
        stage ('remove exiting git folder'){
            sh 'sudo rm -rf /var/www/html/.git'
        }
        stage ('cloning git project'){
            sh 'sudo git clone -b master https://gitlab.com/Sharath029/netflix.git /var/www/html'
        }
    }
}