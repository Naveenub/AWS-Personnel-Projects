# AWS-Personnel-Projects

This is Sample project blog on "How to Launch and connect to an Amazon EC2 MAC instance"

Introduction:-

Amazon EC2 Mac instances enable customers to run on-demand macOS workloads in the cloud for the first time, extending the flexibility, scalability, and cost benefits of AWS to all Apple developers. With EC2 Mac instances, developers creating apps for iPhone, iPad, Mac, Apple Watch, Apple TV, and Safari can provision and access macOS environments within minutes, dynamically scale capacity as needed, and benefit from AWS’s pay-as-you-go pricing.

In this tutorial, I will show how to launch and connect to an Amazon EC2 Mac instance by allocating an Amazon EC2 Dedicated Host. Launching a EC2 Mac instance is a two step process where you first allocate a mac1 Dedicated Host, and then launch a mac1.metal instance onto the Dedicated Host.

There is a 24-hour minimum allocation duration that is applicable to the Dedicated Host itself, not to your mac1.metal instance. 

You can launch and terminate mac1.metal instances as you want on that mac1 Dedicated Host, for example, to switch between a macOS Catalina-based AMI and a macOS Big Sur-based AMI. 

However, once you allocate a mac1 Dedicated Host, you cannot release it until 24 hours later (the minimum lease period is 24 hours for the physical server). Once past those initial 24 hours, you can release the host anytime you want. 

This time period is to comply with the macOS Software Licensing Agreement. As with all Amazon EC2 Dedicated Hosts, you pay per second for the entire duration that Dedicated Host is allocated to your account. 

Instances launched or terminated on that Dedicated Host have no separate charge. Since the minimum host allocation duration for mac1 Dedicated Hosts is 24 hours, by definition, you pay for a minimum 24 hours.
