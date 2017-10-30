pipeline{
		agent any
		
			stages
			{
				stage('bulit')
				{
				    steps{
					sh 'mvn clean package'
					}
					post
					{
						success
						{
							archiveArtifacts artifacts :'**/target/*.war'
						}

					}
				}
				
			}
		
}
