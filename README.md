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


Problem 1: Encryption Time Calculation
A company uses AES-256 encryption to secure its data before uploading it to the cloud. It takes 0.05 seconds to encrypt 1 MB of data.
Q: How long will it take to encrypt 2 TB of data before upload?
To calculate the encryption time for 2 TB (terabytes) of data using AES-256, where 1 MB takes 0.05 seconds,
Step 1: Convert TB to MB
1 TB = 1024 GB
 1 GB = 1024 MB
 So:
 2 TB = 2 × 1024 × 1024 MB = 2,097,152 MB
Step 2: Multiply by encryption time per MB
Time per MB = 0.05 seconds
 Total time = 2,097,152 MB × 0.05 seconds/MB
 = 104,857.6 seconds
It will take approximately 104,857.6 seconds (or ~29.13 hours) to encrypt 2 TB of data using AES-256.


Problem 2:CPU Utilization Efficiency
A VM is allocated 8 vCPUs, but only uses 5.5 vCPUs on average.
Q: What is the CPU utilization efficiency?
CPU Utilization Efficiency
A virtual machine (VM) is provisioned with 8 virtual CPUs (vCPUs). However, on average, it only utilizes 5.5 vCPUs. The objective is to calculate the CPU utilization efficiency.
Solution:
CPU utilization efficiency is calculated using the formula:
CPU Utilization Efficiency=(Total Allocated vCPUsAverage vCPU Usage​)×100
Substituting the given values:

CPU Utilization Efficiency=(5.5/8​)×100=68.75%
Final Answer:
The CPU utilization efficiency is 68.75%.
Problem 3: Network Throughput Efficiency
A cloud server has a maximum bandwidth of 1 Gbps, but during peak hours it only uses 600 Mbps.
Q: What is the network throughput efficiency?
Solution:
Network throughput efficiency is calculated using the formula:
Network Throughput Efficiency=(Actual Throughput/Maximum Bandwidth​)×100
Substituting the given values:
Network Throughput Efficiency=(600/1000)*100=60%
Final Answer:
The network throughput efficiency is 60%.

Problem 4:Energy Efficiency
Two cloud setups process the same workload:
Setup A uses 500W for 2 hours.
Setup B uses 300W for 3.5 hours.
Q: Which setup is more energy-efficient?
Solution:
To compare energy efficiency, we calculate the total energy consumption (in watt-hours) for each setup:
Setup A:
             Energy=500 W×2 hours=1000 Wh
Setup B:
             Energy=300 W×3.5 hours=1050 Wh
Comparison:
Setup A consumes 1000 Wh


Setup B consumes 1050 Wh
Since both setups complete the same workload, the one using less energy is considered more efficient.
Final Answer:
Setup A is more energy-efficient because it uses less total energy (1000 Wh vs. 1050 Wh) to process the same workload.


Problem 5: 
CPU Utilization Efficiency
A physical server has 16 cores and each VM uses 2 cores. CPU utilization is optimal at 75%.
Q: What is the maximum number of VMs that can be efficiently hosted?

Solution:
Step 1: Calculate the number of cores available for efficient use
Efficient cores=75% of 16=0.75×16=12 cores\text{Efficient cores} = 75\% \text{ of } 16 = 0.75 \times 16 = 12\ \text{cores}Efficient cores=75% of 16=0.75×16=12 cores
Step 2: Determine how many VMs can be hosted
Each VM uses 2 cores, so:
Number of VMs= 12/2=6VMs
Final Answer:
The server can efficiently host a maximum of 6 virtual machines at 75% CPU utilization.


