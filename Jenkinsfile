pipeline{
		agent any
		
			stages
			{
				stage('bulit')
				{
				    steps{
					sh 'mvn clean package'
					    
					}
				   steps
					{
						echo 'step2 bulit'
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
