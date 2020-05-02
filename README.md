# AWS Storage Services

Choosing the right AWS storage service for your data means finding the closest match in terms of data availability,
durability, and performance.

**Note:-**

Availability refers to a storage volume’s ability to deliver data upon request. Performance refers to the number of IOPS 
or the amount of throughput (measured in megabytes per second) that the storage volume can deliver.

Amazon offers three broad categories of storage services:
object, block, and file storage.
Each offering is designed to meet a different storage requirement, which gives you flexibility to find the solution 
that works best for your storage scenarios.

# Object storage
**Amazon Simple Storage Service (Amazon S3)** is highly durable, general-purpose object storage that works well for unstructured data sets such as media content. Amazon S3 provides the highest level of data durability and availability on the AWS Cloud. There are three tiers of storage: one each for hot, warm, or cold data. In terms of pricing, the colder the data, the cheaper it is to store, and the costlier it is to access when needed. You can easily move data between these storage options to optimize storage costs:

***Amazon S3 Standard –** The best storage option for data that you frequently access. Amazon S3 delivers low latency
and high throughput and is ideal for use cases such as cloud applications, dynamic websites, content distribution, gaming, 
and data analytics.

***Amazon S3 Standard - Infrequent Access (Amazon S3 Standard - IA) –** Use this storage option for data that you access
less frequently, such as long-term backups and disaster recovery. It offers cheaper storage over time,
but higher charges to retrieve or transfer data.

***Amazon Glacier –** Designed for long-term storage of infrequently accessed data, such as end-of-lifecycle, compliance, 
or regulatory backups. Different methods of data retrieval are available at various speeds and cost.
Retrieval can take from a few minutes to several hours.


# Block storage
**Amazon Elastic Block Store (Amazon EBS)** volumes provide a durable block-storage option for use with EC2 instances.
Use Amazon EBS for data that requires long-term persistence and quick access at guaranteed levels of performance.
There are two types of block storage: solid-state-drive (SSD) storage and hard-disk-drive (HDD) storage.

**SSD storage** is optimized for transactional workloads where performance is closely tied to IOPS. 
  There are two SSD volume options to choose from:

***EBS Provisioned IOPS SSD (io1) –** Best for latency-sensitive workloads that require specific minimum-guaranteed IOPS. 
With io1 volumes, you pay separately for provisioned IOPS, so unless you need high levels of provisioned IOPS,
gp2 volumes are a better match at lower cost.

***EBS General Purpose SSD (gp2) –** Designed for general use and offer a balance between cost and performance.

**HDD storage** is designed for throughput-intensive workloads such as data warehouses and log processing.

There are two types of HDD volumes:
***Throughput Optimized HDD (st1) –** Best for frequently accessed, throughput-intensive workloads.

***Cold HDD (sc1) –** Designed for less frequently accessed, throughput-intensive workloads.


# File storage
**Amazon Elastic File System (Amazon EFS)** provides simple, scalable file storage for use with EC2 instances.
Amazon EFS supports any number of instances at the same time. Its storage capacity can scale from gigabytes to 
petabytes of data without needing to provision storage. Amazon EFS is designed for workloads and applications 
such as big data, media-processing workflows, content management, and web serving. Amazon EFS also supports file 
synchronization capabilities so that you can efficiently and securely synchronize files from on-premises or cloud 
file systems to Amazon EFS at speeds of up to 5 times faster than standard Linux copy tools.

Amazon S3 and Amazon EFS allocate storage based on your usage and you pay for what you use. However, for EBS volumes, you are charged for provisioned (allocated) storage whether or not you use it. The key to keeping storage costs low without sacrificing required functionality is to maximize the use of Amazon S3 when possible and use more expensive EBS volumes with provisioned I/O only when application requirements demand it.
