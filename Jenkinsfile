pipeline{
		agent any
		
			stages
			{
				stage('bulit')
				{
				    steps{
					sh 'mvn clean package'
					}
					
				}
				stage('arch')
				{
					echo 'archive'
				}
			
				
			}
		
}
