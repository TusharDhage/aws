# EC2 VS RDS


> AWS is all about providing computing infra structure in on demand basis. EC2 and RDS are the 2 different service offerings from AWS.
___
**EC2** : Elastic Compute Cloud - On demand Servers either Linux / Windows.

- You are provided with a Instance to which you can RD / SSH.
- You are free to install web server / mail server / db server / app server.
- The instance health is AWS's responsibility and everything inside the instance your responsibility.
___
**RDS** : Relational Database Service

- You are provided with a deployed DB server and you can create the db instance
- You can't do a RD / telnet to connect to the RDS's physical server but you can connect to the RDS instance via clients like SSMS,       MySQL workbench etc or via JDBC / ODBC DB APIs
- You can connect to the RDS instance from any internet enabled client system / application ( provided appropriate firewall rules have     been enabled )
- By extension to the previous point, you can connect to the RDS from your app running in EC2.

**PS** :
You can install a database server in EC2 and use it / configure as you wish; but remember doing that you will hold the responsibility of the DB's uptime 
and health as it becomes an app running in the EC2.
In the RDS, AWS will take care ( manage ) the DB instance health and you just need to concentrate on your data, schema, tables etc.

                                 
