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
steps
{
script{
when {
    expression {
        return env.BRANCH_NAME = 'master';
        }
    }
	}
	
	echo"hi-sample1"
	}
	}
}
}







}
}
