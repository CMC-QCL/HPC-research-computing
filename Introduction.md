# Introduction: HPC Resources

## Local HPC: QCL Server
At the QCL, we have a Dell server machine with 2 CPUs (32 cores) and 512 GB of memory. It is currently repartitioned to serve a database server and a data storage.

## Local HPC: QCL GPU Machine
QCL has an NVIDIA DGX system having four Tesla V100 GPUs. 

| Component                	| Spec                                    	|
|--------------------------	|-----------------------------------------	|
| GPUs                     	| 4X Tesla V100                           	|
| TFLOPS (Mixed precision) 	| 500                                     	|
| GPU Memory               	| 128 GB total system                     	|
| NVIDIA Tensor Cores      	| 2,560                                   	|
| NVIDIA CUDA Cores        	| 20,480                                  	|
| CPU                      	| Intel Xeon E5-2698 v4 2.2 GHz (20-Core) 	|
| System Memory            	| 256 GB RDIMM DDR4                       	|
| Data Storage             	| Data: 3X 1.92 TB SSD RAID 0             	|
| OS Storage               	| OS: 1X 1.92 TB SSD                      	|
| Network                  	| Dual 10GBASE-T (RJ45)                   	|

## Regional HPC Cluster: Laguna

Hosted at the University of Southern California (USC) and managed by the Center for Advanced Research Computing (CARC), Laguna is a state-of-the-art system boasting 2 shared login nodes, 20 compute nodes, and 8 GPU nodes. Through an extensively collaborative effort, the SoCal Regional Research Computing Alliance hopes that access to this advanced computing environment and comprehensive user services will propel local campus research forward exponentially.


|     Category         	|     Function            	|     Qty    	|     Notes                                                                                                                          	|
|----------------------	|-------------------------	|------------	|------------------------------------------------------------------------------------------------------------------------------------	|
|     Public facing    	|     Login node          	|     1      	|     Dual AMD EPYC 9354 3.25GHz (32C/64T) w/   384 GB                                                                               	|
|     Computing        	|     Compute node        	|     16     	|     Dual AMD EPYC 9554 3.1GHz (64C/128T,   256M Cache) CPU     384 GB memory per node                                              	|
|     Computing        	|     GPU node            	|     8      	|     Dual EPYC 9354 3.25GHz (32C) + Dual   Nvidia L40s GPU (18K CUDA cores, 568 Tensor cores, and 48GB GDDR6 mem) w/   768GB mem    	|
|     Network          	|     Interconnection     	|     N/A    	|     Mellanox CX-7 InfiniBand NDR (200 Gbps)                                                                                        	|
|     Storage          	|     /home & /project    	|     4      	|     Dual AMD Epyc 9224 2.5GHz (24C/48T) w/192GB memory 

12 x 15TB NVMe SSD (4 x 180TB = 720TB)                                  	|

## National Supercomputers: ACCESS

ACCESS is a collection of integrated advanced digital resources and services that provide easy access to the most advanced computational resources and scientific research support in the world. QCL has two Campus Champions who are trained to help local users utilize national supercomputing resources available through the NSF Access program. From various national supercomputing facilities, QCL has awarded a large number of computing hours for testing and developing scientific applications (see below).

| Name                      	| Facility                            	| SU (Core Hours)   	|
|---------------------------	|-------------------------------------	|-------------------	|
| ANVIL CPU                 	| Purdue                              	| 100,000 SUs       	|
| ANVIL GPU                 	| Purdue                              	| 1,000 SUs         	|
| Bridges Extreme Memory    	| PSC                                 	| 1,000 Core Hours  	|
| Bridges-2 GPU             	| PSC                                 	| 2,500 GPU Hours   	|
| Bridges-2 Regular Memory  	| PSC                                 	| 50,000 SUs        	|
| DARWIN Compute Node       	| UD                                  	| 20,000 SUs        	|
| DARWIN GPU                	| UD                                  	| 400 SUs           	|
| EXPANSE CPU               	| SDSC                                	| 50,000 Core Hours 	|
| EXPANSE GPU               	| SDSC                                	| 2,500 GPU Hours   	|
| Jetstream                 	| Indiana U                           	| 50000 SUs         	|
| KyRIC Large Memory Nodes  	| Kentucky Research Informatics Cloud 	| 1,000 Core hours  	|
| OSG                       	| Multiple                            	| 200,000 SUs       	|
| Rockfish - GPU            	| Johns Hopkins                       	| 500 GPU hours     	|
| Rockfish - Large Memory   	| Johns Hopkins                       	| 1,000 Core hours  	|
| Rockfish - Regular Memory 	| Johns Hopkins                       	| 20,000 Core hours 	|
| Stampede2                 	| TACC                                	| 1,600 Node Hours  	|

The Service Unit (SU) is like a currency used to run an application on supercomputers. Supercomputer users are charged by SUs (hours of runtime on one core). For example, if an application ran on 100 cores for 10 hours, 1,000 SUs will be deducted from your account.

The Campus Champion allocations can be used to test computational research applications. To test out the supercomputers, please make an appointment with one of the CMC Campus Champions (email: qcl@cmc.edu).
