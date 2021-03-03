pipeline{
agent any;
tools{
  maven 'maven3.6.3'
}
stages{
    stage('CheckOutCode'){
	 steps{
	  git branch: 'main', credentialsId: 'a8a1f9d1-c5c2-46d7-b260-d46185da67fa', url: 'https://github.com/vasujenkinsorg/mavenwebapplication.git'
	 }
	}
	 stage('Build'){
	 steps{
	  sh "mvn clean package"
	 }
	}
}

}
