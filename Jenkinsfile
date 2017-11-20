pipeline{
		agent any
		
			stages
			{
				stage('bulit')
				{
				    steps{
					sh 'mvn clean package1'
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
