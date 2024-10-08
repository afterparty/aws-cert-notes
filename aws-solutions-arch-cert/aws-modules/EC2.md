# EC2

Elastic Compute Cloud

provisioned virtual machines in the cloud

## EC2 pricing models

* on demand - fixed rate by the hour with no commitment

* reserved - provides you with a capacity reservation and off a significant discount on the hourly charge for an instance. Contract Terms are 1 year or 3 years

* spot - enables you to bid watever price you want for instance capacity, providing for even greater savings if your applications have flexible start and end times

* dedicated hosts - physical ec2 server dedicated for your use. dedicated hosts can help you reduce costs by allowing you to use your existing server-bound software licenses

on demand - low cost flexible without any upfront payment or long term commitment

applications with short term spiky or unpredictable workloads that cannot be interrupted

applications being developed or tested on ec2 for the first time

reserved pricing - applications with steady state or predictable usage

applications that require reserved capacity

users make upfront payments to reduce their total computing costs even further

standard reserved instances - 75% off on demand instances more up front paid the longer the contract the greater the discount

convertible reserved instance - covers 54% off on demand capability to change the attributes of the RI as long as the exchange results in the creation of RI of equal or greater value

scheduled reserved instances - launch instances during a time window

spot pricing - applications that have a flexible start and end times

applications that are only feasible at very low compute prices

users with urgent computing needs

dedicated hosts - useful for regulatory requirements that may not support mult tenant virtualization

great for licensing which does not support mult-tenancy or cloud deployments

can be purchased On-Demand hourly

can be purchased as reserved at 70 percent of on demand

## EC2 instances

    lots of ec2 instance types

    f1 fpga

    i3 high speed storage

    g3 graphics intensive

    h1 high disk throughput

    t3 lowest cost general purpose

    d2 dense storage

    r5 memory optimized

    m5 general purpose

    c5 compute optimized

    p3 gpu

    x1 memory optimized 

    z1d high computer capacity and high memory footpritn

    a1 arm based workloads

    u-6tb1 bare metal

    mnemonic fight dr mcpyxz au

AMI - Amazon Machine Image is a proconfigured that includes operating system, possible applications to be pre-installed on that instance upon launch and other configurations

EC2 can do the following:

* Provision and launch one or more EC2 instances in minutes
* Stop or shut down EC2 instances when you finish running a workload
* pay by the hour or second for each instance types (min 60 seconds)

To Create an EC2 instance you must define:

* __Hardware specifications__: CPU, memory, network, and storage
* __Logical configurations__: Networking location, firewall rules, authentication and the operating system

use a EC2 instance to create an AMI

EC2 Naming Convention - c5n.xlarge

* __First Position__ - the first position c indicates the instance family. This indicates that this instance belongs to the compute optimizied family
* __Second Position__ - the second position 5 indicates the generation of the instance. This instance belongs to the fifth generation of instances
* __Remaining letter before the period__ - in this case n indicates additional attributes such as local NVMe storage
* __After the period__ - after the period xlarge indicates the instance size it's xlarge

Instance families

* General purpose
* Computer optimized
* Memory optimized
* Accelerating computing
* Storage optimized
* HPC optimizer

EC2 Lifecycle

launch state
pending state - vm booting up
running state

* reboot
* stopping -> stop instance
* stop-hibernate
* terminate
