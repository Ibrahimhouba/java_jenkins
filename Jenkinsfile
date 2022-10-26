node {
    stage('clone') {
        git 'https://github.com/Ibrahimhouba/java_jenkins.git'

}
    stage('build') {
   sh 'javac affichage.java'
}
    stage('run') {
        sh 'java affichage'
     
   stage('test') {
       
        sh 'result=`ps aux | grep -i "affichage.java" | grep -v "grep" | wc -l`; if [ $result -ge 0 ]; then echo "ERROR >> KO "; fi'
   }

}
}
