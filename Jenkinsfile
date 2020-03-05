pipeline
{
agent any
  triggers {
    pollSCM('* * * * * ') // Enabling being build on Push
  }
tools
{
git 'Default'
}
environment {
        
		Branch_Name = "${env.BRANCH_NAME}"
	        Imagebranch = "${env.JOB_NAME}"
    }
stages
{
stage("Creating backup for binary images")
{
steps
{
echo"hi-sample1"
}
}
stage("Build")
{

when{
    branch 'master'
  }
  steps {
    echo 'run this stage - ony if the branch is master branch::"${Imagebranch}"'
  }
}
stage("Deploy")
{

when{
    branch 'master'
  }
  steps {
    echo 'Deploy stage - ony if the branch is master branch'
  }
}
}
}
