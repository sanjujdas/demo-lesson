node ('app1'){
    def app

    stage('Clone repository') {
          /* Let's make sure we have the repository cloned to our workspace */

        checkout scm
    }
    stage('Deploy to nginx') {
        sh "rm -rf /var/www/html/*"
        sh "cp index.html /var/www/html/"
        sh "systemctl restart nginx"
        }

}