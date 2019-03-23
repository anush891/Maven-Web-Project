node{

stage("checkout"){
checkout scm
}

stage("build"){
bat 'mvn clean install'
}

stage("deploy to sonarqube"){
bat 'mvn sonar:sonar'
}

stage("deploy to nexus"){
bat 'mvn clean deploy'
}

stage("deploy to tomcat"){
bat 'copy **\*.war E:\Softwares\apache-tomcat-8.5.38\apache-tomcat-8.5.38\webapps\'
}

}
