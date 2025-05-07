### Name: Divya R V
### Reg no: 21222300005

# CASE-STUDY-

Case Study Title: Resource Allocation and Cost Optimization in an OpenStack Private Cloud

Case Overview:

ABC Cloud Services runs a private cloud using OpenStack to host virtual machines (VMs) for internal development, testing, and production workloads. Their cloud infrastructure comprises:

5 Compute Nodes, each with:
64 vCPUs
256 GB RAM
2 TB SSD storage
OpenStack Services Deployed:
Nova (Compute)
Neutron (Networking)
Cinder (Block Storage)
Glance (Image Management)
Keystone (Identity)
Horizon (Dashboard)
Heat (Orchestration)

They are considering expanding their cloud but want to first evaluate current capacity usage, VM density, and cost efficiency. The goal is to calculate whether their resource usage aligns with business needs and how to optimize it.

Case Study Questions – OpenStack Calculation in Cloud Computing

1. Resource Utilization:

Based on the current infrastructure, what is the total available compute capacity in terms of:
Total vCPUs
Total RAM
Total storage

2.Storage Allocation:

Given 10 TB of total block storage across the cloud, how many VMs can be supported if:
a) Each VM is allocated 100 GB block storage
b) Snapshot storage consumes 20% extra on average

**SOLUTIONS:**

1. Resource Utilization:
Based on the current infrastructure, what is the total available compute capacity in terms of:

Total vCPUs

Total RAM

Total storage

Solution:

For 5 compute nodes, each with:

64 vCPUs

256 GB RAM

2 TB SSD storage

We can calculate the total available resources by multiplying the values for each node by the number of nodes (5 nodes):

Total vCPUs:
Total vCPUs = 64vCPUs/node × 5 nodes = 320 vCPUs

Total RAM:
Total RAM = 256 GB/node × 5 nodes = 1,280 GB = 1.28 TB

Total Storage:
Total Storage = 2 TB/node × 5 nodes = 10 TB

Thus, the total available resources are:

320 vCPUs
1.28 TB RAM
10 TB storage

2. Storage Allocation:
Given 10 TB of total block storage across the cloud, how many VMs can be supported if:

a) Each VM is allocated 100 GB block storage
b) Snapshot storage consumes 20% extra on average

Solution:

a) Without considering snapshot storage:

Each VM is allocated 100 GB of block storage. To calculate how many VMs can be supported:

Number of VMs = Total Storage/Storage per VM = 10,000 GB/100 GB/VM = 100 VMs

b) Considering snapshot storage, which consumes 20% extra:

The effective storage needed per VM is increased by 20% due to snapshot storage:

Storage per VM with snapshots=100 GB×1.2=120 GB
Now, calculate the number of VMs that can be supported considering the increased storage requirement:
Number of VMs with snapshots= 
120 GB/VM
10,000 GB
 =83.33≈83 VMs
Thus, the number of VMs that can be supported are:

Without snapshots: 100 VMs

With snapshots: 83 VMs
