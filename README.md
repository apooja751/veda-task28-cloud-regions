# Task 28: Understand and Configure Cloud Regions

## Veda Technology — Cloud Computing Internship

### Overview
This task explores AWS geographic regions and Availability Zones by comparing the Asia Pacific (Mumbai) and Asia Pacific (Singapore) regions. The objective is to understand regional infrastructure, compare EC2 instance options, and identify factors that influence cloud region selection.

### Objectives
- Understand AWS Regions and Availability Zones.
- Inspect EC2 instance configuration options in two regions.
- Compare regional subnet and Availability Zone information.
- Understand latency, availability, compliance, and pricing considerations.
- Identify why organizations deploy workloads in different regions.

### Tools and Services
- Amazon Web Services (AWS)
- Amazon EC2
- Amazon VPC
- AWS Management Console
- Ubuntu Server
- GitHub

### Region Comparison

| Feature | Mumbai | Singapore |
|---|---|---|
| AWS Region | Asia Pacific (Mumbai) | Asia Pacific (Singapore) |
| Region code | `ap-south-1` | `ap-southeast-1` |
| Operating system inspected | Ubuntu Server | Ubuntu Server |
| Instance type inspected | `t3.micro` | `t3.micro` |
| Subnets observed in the account | 3 | 3 |
| Availability Zones represented in the observed subnet list | 3 | 3 |
| Geographic consideration | Suitable for workloads serving users in India | Suitable for workloads serving users in Southeast Asia |

*Note: Subnet counts reflect the console observations during this exercise and do not represent the total subnet or Availability Zone capacity of either AWS Region. Instance type inspection does not guarantee that an instance is available for launch or free of charge.*

### Understanding Regions and Availability Zones

**AWS Region:** A separate geographic area where AWS provides cloud services.

**Availability Zone:** An isolated location within an AWS Region, designed to support workload availability and resilience.

Deploying workloads across multiple Availability Zones can help improve fault tolerance. Deploying across multiple Regions can support disaster recovery, geographic reach, and certain data-residency requirements.

### Region Selection Considerations

1. **Latency:** Choose a region close to the application's users when low response times are important.
2. **Availability:** Consider the required services and resilience architecture.
3. **Compliance:** Verify applicable data-residency and regulatory requirements.
4. **Pricing:** Compare regional service prices and account-specific free-tier eligibility.
5. **Service availability:** Confirm that the required instance types and AWS services are available in the chosen region.

### Screenshots and Evidence

Save the screenshots in a folder named `screenshots/` and use these filenames:

1. `Task28_01_Mumbai_EC2_Instance_Options.png`
2. `Task28_02_Singapore_EC2_Instance_Options.png`
3. `Task28_03_Singapore_Availability_Zones.png`
4. `Task28_04_Singapore_AZ_Details.png`
5. `Task28_05_Mumbai_AZ_Details.png`

### Implementation Summary

The AWS Management Console was used to inspect EC2 configuration options in Mumbai and Singapore and to examine existing subnet Availability Zone assignments in both regions. No new EC2 instances or subnets were created for this comparison.

### Conclusion

The exercise demonstrates how AWS Regions and Availability Zones support geographic distribution and resilient cloud architecture. The appropriate region should be selected according to user location, latency, service availability, compliance requirements, resilience objectives, and cost.
