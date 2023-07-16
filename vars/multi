def newGit(repo)
{
  git "${repo}"
}

def newMaven()
{
  sh "mvn package"
}

def newDeploy(workspace,ip,context)
{
  sh "scp ${workspace}/webapp/target/webapp.war ubuntu@${ip}:/var/lib/tomcat9/webapps/{context}.war"
}

def newTesting(workspace)
{
  sh "java -jar ${workspace}/testing.jar"
}
