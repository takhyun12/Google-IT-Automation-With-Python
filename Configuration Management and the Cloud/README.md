# Configuration Management and the Cloud

Certificate of the course that is offered at Coursera and Google.

#### Author: Tackhyun Jung

#### Status: Completed

This repository is created to keep track of [Configuration Management and the Cloud](https://www.coursera.org/learn/configuration-management-cloud) provided by Coursera. 
This educational program is developed by Google and designed to teach how to program with python Programming.

![Certification](https://user-images.githubusercontent.com/41291493/109306625-c6200180-7882-11eb-8995-0e64e7f31d07.png)

## Learning Objectives
* Learn how to use Puppet, the current industry standard for configuration management
* Learn about the benefits and challenges of moving services to the Cloud
* Learn the best practices for handling hundreds of virtual machines running in the Cloud
* Learn how to install Puppet on your computer and how to use a simple test setup to check your rules work as expected
* Learn how to configure the typical client-server set-up with Puppet clients connecting and authenticating to the Puppet server to get the rules that they should apply
* Learn how to use testing techniques and releasing best practices to safely deploy changes to clients of our configuration management system
* Learn how cloud deployments can help us quickly scale our services
* Learn the differences between when running IT infrastructure on-premise versus running it in the cloud
* Learn how we can use a variety of different tools to manage instances running in the cloud
* Understand and explain the different types of storage available
* Explain the difference between round robin DNS and sticky sessions
* List the different types of integration testing that are available
* Understand and explain the concept of SLAs
* Troubleshoot and debug a system without being physically present
* Understand what a rollback is and how they can help in a system failure
* Understand how primary and secondary instances can help in a disaster recovery situation

```
# Peppet
With Puppet’s automation, new applications and changes can be released simultaneously and with no downtime.

# 5 ways Puppet will make a developer’s life easier
1. It brings consistency to your servers
2. It’s reliable
3. Faster time to deployment
4. It’s easy to add more servers
5. More time to focus on what you love to do

# What benefits can we gain by using automation to manage our configuration?
Consistency
Reliability
Scalability

# What is templating?
The process of capturing the entire system configuration to enable us to reproduce virtual machines

class machine_info {
  if $facts[kernel] == "windows" {
       $info_path = "C:\Windows\Temp\Machine_Info.txt"
   } else {
       $info_path = "/tmp/machine_info.txt"
   }
 file { 'machine_info':
       path => $info_path,
       content => template('machine_info/info.erb'),
   }
}

class packages {
   package { 'python-requests':
       ensure => installed,
   }
   if $facts[os][family] == "Debian" {
     package { 'golang':
       ensure => installed,
     }
  }
   if $facts[os][family] == "RedHat" {
     package { 'nodejs':
       ensure => installed,
     }
  }
}

Machine Information
-------------------
Disks: <%= @disks %>
Memory: <%= @memory %>
Processors: <%= @processors %>
Network Interfaces: <%= @interfaces %>
}
```

## Credit

* [Certification-Link](https://www.coursera.org/account/accomplishments/verify/D6C447R8GSCD)
