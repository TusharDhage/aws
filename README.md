# DATABASE-RDS

**Amazon Relational Database Service Documentation**

Amazon Relational Database Service (Amazon RDS) is a web service that makes it easier to set up, 
operate, and scale a relational database in the cloud. It provides cost-efficient,
resizable capacity for an industry-standard relational database and manages common database administration tasks.

**Overview of Amazon RDS**

Why do you want a managed relational database service? Because Amazon RDS takes over many of the
difficult or tedious management tasks of a relational database:
• When you buy a server, you get CPU, memory, storage, and IOPS, all bundled together. With Amazon
RDS, these are split apart so that you can scale them independently. If you need more CPU, less IOPS,
or more storage, you can easily allocate them.
• Amazon RDS manages backups, software patching, automatic failure detection, and recovery.
• To deliver a managed service experience, Amazon RDS doesn't provide shell access to DB instances. It
also restricts access to certain system procedures and tables that require advanced privileges.
• You can have automated backups performed when you need them, or manually create your own
backup snapshot. You can use these backups to restore a database. The Amazon RDS restore process
works reliably and efficiently.
• You can get high availability with a primary instance and a synchronous secondary instance that you
can fail over to when problems occur. You can also use MySQL, MariaDB, or PostgreSQL read replicas
to increase read scaling.
• You can use the database products you are already familiar with: MySQL, MariaDB, PostgreSQL, Oracle,
Microsoft SQL Server.
• In addition to the security in your database package, you can help control who can access your RDS
databases by using AWS Identity and Access Management (IAM) to define users and permissions. You
can also help protect your databases by putting them in a virtual private cloud.


***DB Instances***

The basic building block of Amazon RDS is the DB instance. A DB instance is an isolated database
environment in the AWS Cloud. Your DB instance can contain multiple user-created databases. You
can access your DB instance by using the same tools and applications that you use with a standalone.


database instance. You can create and modify a DB instance by using the AWS Command Line Interface,
the Amazon RDS API, or the AWS Management Console
Each DB instance runs a DB engine. Amazon RDS currently supports the MySQL, MariaDB, PostgreSQL,
Oracle, and Microsoft SQL Server DB engines. Each DB engine has its own supported features, and
each version of a DB engine may include specific features. Additionally, each DB engine has a set of
parameters in a DB parameter group that control the behavior of the databases that it manages.
