# DevInfos - *by ZULEE*

## VIRTUALIZATION

-Use docker in Hyper-V Guest OS

  Run this command in PS as an administrator
  
  `Set-VMProcessor -VMName ***VM_NAME*** -ExposeVirtualizationExtensions $true`
  

## DOCKER

- Connect form host with MSSMS ot MS SQL server running in a Docker container:
  
  Start docker container drom CMD:  `docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=SqLP@ssw0rd" -p 1433:1433 --name sql1 --hostname sql1 -d mcr.microsoft.com/mssql/server:2022-latest`
  
  Enter `127.0.0.1,1433` in the connect window of the MSSMS.
