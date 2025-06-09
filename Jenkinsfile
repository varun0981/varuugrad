pipeline{
	agent any 
	tools{
		gradle 'Gradle'
		jdk 'JDK'
	}
	stages{
		stage('checkout'){
		steps{
			git branch :'master',url:''
		}
	}
		stage('Build'){
		steps{
			sh'gradle build'
		}
	}
		stage('Test'){
		steps{
			sh'gradle test'
		}
	}
		stage('Run Application'){
		steps{
			sh'gradle run'
		}
	}
}
}

		
