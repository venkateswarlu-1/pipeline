
pipeline {
agent any
 
tools{
maven 'maven361'
jdk 'jdk'
git 'git'
}

stages {
stage('Git Clone')
{
 steps { git url: 'https://github.com/jenkins-docs/simple-java-maven-app.git'
      }
}


        stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean package'
           
        }
}

}
}
