# S3 Storage Classes 
Amazon S3 (Simple Storage Service) offers several storage classes designed to meet different use cases based on access frequency, retrieval time, and cost. Here are the main S3 storage classes:

1. **Amazon S3 Standard (S3 Standard)**
2. **Amazon S3 Intelligent-Tiering (S3 Intelligent-Tiering)**
3. **Amazon S3 Express One Zone**
4. **Amazon S3 Standard-Infrequent Access (S3 Standard-IA)**
5. **Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA)**
6. **Amazon S3 Glacier Instant Retrieval**
7. **Amazon S3 Glacier Flexible Retrieval (Formerly S3 Glacier)**
8. **Amazon S3 Glacier Deep Archive**
9. **S3 Outposts**

### **1. S3 Standard**:

- Designed for frequently accessed data.
- Low latency and high throughput performance.
- Ideal for a wide variety of use cases including cloud applications, dynamic websites, content distribution, and big data analytics.
- No retrieval fees and a higher storage cost compared to other classes.

### **2. S3 Intelligent-Tiering**:

- Optimizes costs by automatically moving data to the most cost-effective access tier without performance impact or operational overhead.
- Suitable for data with unknown or changing access patterns.
- Two access tiers: frequent and infrequent.
- Small monthly monitoring and automation fee.

### **3. S3 Standard-IA (Infrequent Access)**:

- Lower storage cost for data that is less frequently accessed but requires rapid access when needed.
- Suitable for long-term storage, backups, and disaster recovery.
- Retrieval fee per GB.

### **4. S3 One Zone-IA**:

- Lower cost option for infrequently accessed data that does not require multiple Availability Zone (AZ) data resilience.
- Suitable for secondary backups or easily re-creatable data.
- Lower cost than S3 Standard-IA but with lower durability.

### **5. S3 Glacier**:

- Low-cost storage for data archiving.
- Retrieval times range from minutes to hours.
- Suitable for long-term backups, digital preservation, and data archiving.
- Very low storage cost with a retrieval fee.

### **6. S3 Glacier Deep Archive**:

- Lowest-cost storage class, designed for long-term data retention.
- Retrieval times of 12 hours or more.
- Ideal for data that is rarely accessed and requires long-term retention.
- Lowest storage cost with a higher retrieval fee compared to S3 Glacier.

### **7. S3 Outposts**:

- Extends S3 to on-premises environments.
- Same APIs, tools, and features available in AWS regions.
- Useful for workloads that require low latency or local data processing.

### **8. S3 Reduced Redundancy Storage (RRS)** (deprecated for new use):

- Lower durability (99.99%) compared to other S3 classes.
- Was designed for non-critical, reproducible data.

### **9. S3 Outposts**

- S3 Object compatibility and bucket management through the S3 SDK
- Designed to durably and redundantly store data on your Outposts
- Encryption using SSE-S3 and SSE-C
- Authentication and authorization using IAM, and S3 Access Points
- Transfer data to AWS Regions using AWS DataSync
- S3 Lifecycle expiration actions
