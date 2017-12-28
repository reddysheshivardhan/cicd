pipeline
{
  agent any
  triggers
  {
    pollSCM('* * * * *')
  }
  stages
  {
  stage('onetes')
  {
    steps
    {
      input 'Aprroval test'
      build 'Dev'
    }
  }
  }
}
