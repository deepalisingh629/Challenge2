- To retrive metadata of an instance, we can use below methods-(tried for linux)
1. Login to Azure Vm
2. jq utility was not available so had to install it using sudo apt install jq -y
3. Executed this command - 
curl -s -H Metadata:true --noproxy "*" "http://169.254.169.254/metadata/instance?api-version=2021-02-01" | jq
