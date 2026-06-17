pipeline{
agent any
tools{
maven 'maven'
}
stages{
stage('checkout'){
steps{
checkout scm
}
}
stage('build and test'){
steps{
sh 'mvn clean package'
}
}
stage('run'){
steps{
sh 'java -jar target/lab1-1.0-SNAPSHOT.jar'
}
}
}
}

