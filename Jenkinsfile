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
      build 'Dev'
    }
  }
  }
}
