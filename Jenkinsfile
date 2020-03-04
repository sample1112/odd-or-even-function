pipeline
{
agent any
  triggers {
    pollSCM('* * * * *') // Enabling being build on Push
  }
tools
{
git 'Default'
}
stages
{
stage("Creating backup for binary images")
{
steps
{
echo"hi-sample1 sample branch"
}
}
}
}
