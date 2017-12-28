pipeline
{
  agent any
  triggers
  {
    pollSCM('* * * * *')
  }
  stages
  {
  stage('one')
  {
    steps
    {
      build 'Dev'
    }
  }
  }
}
