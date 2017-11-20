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
					steps
					{
					echo 'archive'
						archiveArtifacts '**/target/*.war'
					
					}
				}
			
				
			}
		
}
