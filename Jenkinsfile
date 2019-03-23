node {

stage("checkout"){

// git branch: 'stage', credentialsId: '36b14edf-cce8-4466-a581-055d8531c682', url: 'https://github.com/anush891/Maven-Web-Project.git'
 
  checkout scm
}

stage("build"){

bat 'mvn clean deploy'

}
}
