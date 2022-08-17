# Introduction

## What?

Infrastructure as code uses the idea of having a full declarative description of the components
that should be running at any given time, from the name of the machine to the last package
installed on it. A tool then parses this description file and corrects any discrepancies observed,
such as updating a firewall rule, changing an IP address, attaching more disk, or whatever is needed. 
If the resource disappears, it’s brought back to life to match the desired state. 

Here we use AWS and Terraform.

## Why?

* Maintenance takes little time and we can focus on the red teaming itself.
* Automating the server set up process helps in exploring current DevOps methodology to better understand what to look 
for once we are in a similar environment.
* Terraform is open source and [supports a number of cloud providers](https://registry.terraform.io/browse/providers), 
which makes it the best choice if you chose an alternative provider that accepts Zcash.

## How?

* [AWS](aws.md)
* [Download Terraform in bouncing server](terraform.md)
* [Spawn containers](containers.md)






