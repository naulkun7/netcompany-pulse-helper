[How to reset a data model - Overview](https://source.netcompany.com/tfs/NC02/Pulse%20Docs/_wiki/wikis/O0300%20-%20Developer%20Guide/4338/How-to-reset-a-data-model)

![[Pasted image 20250711160542.png]]

**Replace this step by**
- kubectl get deploy -n dev01 --no-headers -o custom-columns=":metadata.name" | % { $d=$_.Trim(); if($d -eq 'strimzi-kafka-kowl' -or $d -eq 'azure-devops-agent-dev01'){ Write-Host "Skipping $d" } else { kubectl scale deploy $d -n dev01 --replicas=0 } }





[Tool.Configuration.Initialize - Repos](https://dev.azure.com/nc-pulse/Pulse/_git/Tool.Configuration.Initialize)
Tools\Tool.Configuration.Initialize\Properties\launchSettings.json
```
"cist initialize -c luan": 
{
  "commandName": "Project",
  "commandLineArgs": "initialize -c --skip-master-data --skip-observable-entity --skip-user-profile --skip-permission-model",
  "environmentVariables": {
    "RootFolder": "C:\\Developer\\ARLA\\ARLA.Configuration.Initialize",
    "ApiUrl": "https://api.arla-dev01.pulse.netcompany.com/",
    "ApiToken": ""
  }
}
```
