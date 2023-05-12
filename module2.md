# Module 2

### 2023-05-12

#### Amazon Elastic Compute Cloud (EC2)
* EC2 instances can be requested as you go (pay for running instances, not stopped or paused)
* multitenancy - sharing underlying hardware between VMs i.e., sharing host with multiple other instances (VMs), hypervisor shares resources
* multiple EC2 instances on same server possible, but they are secure from each other
* configs: Windows/Linux, dbs, software, internal business apps etc.
* instances resizable -> vertical scaling of instances
* CaaS - compute as a service


#### EC2
* Launch - configs
* Connect - to the instance
* Use - run commands, install software, I/O files etc.
* EC2 Instance types vary across CPU, memory capacity, storage, networking capacity
    - **general purpose** - well balanced
    - **compute** optimised e,g. HPC, scientific modelling, gaming servers
    - **memory** aka accelerated optimised e.g. graphics processing, float calculations, data pattern matching
    - **storage** optimised e.g. needing lots of storage, high sequential I/O (measured using IOPS) to large datasets on local storage like file systems, data warehousing, OLTP systems


#### Pricing
* various pricing schemes and ways to save e.g., savings plans, reserved instances, spot, and dedicated hosts (most $$$)

#### Scaling


   
