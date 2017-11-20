pipeline
{
  agent any
  trigger
  {
    pollSCM('* * * * *')
  }
  stages
  {
  stage('one')
  {
    steps
    {
      build 'job2'
    }
  }
  }
}
