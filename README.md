# Cloud-Computing-Performance-Testing

### Part 1: Virtual Machines Performance Test

Setup

Create a set of virtual machines ( 2 VMs).
Connect them using a virtual switch and local IPs.
Allocate limited resources to each VM (2 CPUs, 2GB of RAM and 15Gb of storage).
Performance Tests

CPU Test: Use HPC Challenge Benchmark for high-performance computation benchmarking (availabe for Ubuntu).
General System Test: Use stress-ng  to evaluate CPU and memory performance.
Disk I/O Test: Use IOZone to test local filesystem I/O. 
Network Test: Use tools like iperf to measure network throughput and latency between VMs.

### Part 2: Containers Performance Test

Setup

Create a Docker Compose file to define a set of containers (2 containers).
Connect the containers using internal Docker network.
Limit resources for each container using Docker Compose options (2 CPUs and 2GB of RAM).
Performance Tests

CPU Test: Run HPC Challenge Benchmark for CPU performance and/or stress-ng  for general system performance.
Disk I/O Test: Use IOZone to test local filesystem performance within containers.
Network Test: Use iperf to measure network throughput between containers.
Final Comparison

#### Analyze
Compare the performance results across VMs, containers
Discuss the impact of resource allocation, virtualization overhead, and network/file system efficiency.
Deliverables

#### Report containing:
Steps for setting up VMs and containers.
Performance metrics (HPL, stress-ng, disk I/O, and network throughput).
Observations and analysis of the performance tests.
