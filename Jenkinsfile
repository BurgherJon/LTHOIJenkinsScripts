#!groovy

//Checkout the LTHOI Code
echo 'Checking out the code.'

node
{
	checkout([$class: 'GitSCM', branches: [[name: '*/master']], 	doGenerateSubmoduleConfigurations: false, extensions: [], 	submoduleCfg: [], userRemoteConfigs: [[credentialsId: 	'f233d4ba-e920-4b3a-a336-9310eeeae298', url: 	'https://github.com/BurgherJon/leavethehouseoutofit']]])
}

echo 'Done'