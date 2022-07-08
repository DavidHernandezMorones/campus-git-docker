# Git & Docker

## Docker

> docker pull hello-world

> docker run hello-world

## Docker/SQL Server

> docker pull mcr.microsoft.com/mssql/server:2022-latest

La carpeta mssql debe estar creada en el home-directory del usuario con sus respectivas carpetas de data, secrets y log
> docker run -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=SQLd0cker!" -p 9001:1433 -v c:\Users\%USERNAME%\mssql\sqldata:/var/opt/mssql/data -v c:\Users\%USERNAME%\mssql\sqllog:/var/opt/mssql/log -v c:\Users\%USERNAME%\mssql\sqlsecrets:/var/opt/mssql/secrets -d mcr.microsoft.com/mssql/server:2022-latest
