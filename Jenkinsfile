#!groovy

echo 'Executing from Git'

node
{
	//Checkout the code
	echo 'Checkout code'
	checkout([$class: 'GitSCM', branches: [[name: '*/master']], 	doGenerateSubmoduleConfigurations: false, extensions: [], 	submoduleCfg: [], userRemoteConfigs: [[credentialsId: 	'f233d4ba-e920-4b3a-a336-9310eeeae298', url: 	'https://github.com/BurgherJon/leavethehouseoutofit']]])

	//Build the code
	build job: 'LTHOI Build', quietPeriod: 0
}

echo 'Done'