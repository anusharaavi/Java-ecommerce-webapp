pipeline
{
  agent
  {
    docker
    {
      image 'abhishekf5/maven-abhishek-docker-agent:v1'
      args '--user root -v /var/run/docker.sock:/var/run/docker.sock'
    }
  }
  stages
  {
    stage (build and test)
    {
      steps
      {
        sh 'ls -ltr'
        sh 'mvn clean package'
      }
    }
   }
}
