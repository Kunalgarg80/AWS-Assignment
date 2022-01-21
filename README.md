# AWS-Assignment

KUNAL GARG
Emp.Id- 1729

What is CIDR Block ?

Classless Inter-Domain Routing (CIDR) block basically is a method for allocating IP addresses and IP routing. When you create a network or route table, you need to specify what range are you working in. "0.0.0.0" means that it will match to any IP address. Some IP addresses are specific, like 10.0.0.0, which will match to any IP address beginning with 10. With any IP address range, you can be more specific by using a suffix(something like /32 from your example). These allow the notation to specify number of bits to be used from Prefix(actual IP-range like 10.0.0.0). It represents the bit length of the subnet mask, as indicated above. The subnet mask is like masking when painting. You place a mask over what you DO NOT want to paint on.

For example, 10.10.0.0/16 will have 256 * 256 IP address in its range.

- Some of the IP address in a range are reserved for various purposes. According to AWS VPC documentation, following are the reserved IP addresses-

10.0.0.0: Network address.
10.0.0.1: Reserved by AWS for the VPC router.
10.0.0.2: Reserved by AWS. The IP address of the DNS server is always the base of the VPC network range plus two; however, we also reserve the base of each subnet range plus two. For VPCs with multiple CIDR blocks, the IP address of the DNS server is located in the primary CIDR. For more information, see Amazon DNS Server.
10.0.0.3: Reserved by AWS for future use.
10.0.0.255: Network broadcast address. We do not support broadcast in a VPC, therefore we reserve this address.

What is Roles?

IAM role is an IAM entity that defines a set of permissions for making AWS service requests. IAM roles are not associated with a specific user or group. Instead, trusted entities assume roles, such as IAM users, applications, or AWS services such as EC2.


what is EC2 , why we use ?

Amazon Elastic Compute Cloud (Amazon EC2) provides scalable computing capacity in the Amazon Web Services (AWS) Cloud. Using Amazon EC2 eliminates your need to invest in hardware up front, so you can develop and deploy applications faster. You can use Amazon EC2 to launch as many or as few virtual servers as you need, configure security and networking, and manage storage. Amazon EC2 enables you to scale up or down to handle changes in requirements or spikes in popularity, reducing your need to forecast traffic.

Amazon EC2 provides different instance types to enable you to choose the CPU, memory, storage, and networking capacity that you need to run your applications.
