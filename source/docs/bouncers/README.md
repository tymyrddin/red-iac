# Introduction

## What?

Bouncing servers are virtual hosts set up anonymously, to SSH into after connecting to via Tor or a VPN, and trust to 
interact with the rest of our attack infrastructures, but never interact with the target. Delete and re-create 
bouncing servers every few weeks. Limitation is the payment solution supported by the providers.

## Why?

* Bouncing servers are used to host management tools like Terraform, Docker, and Ansible to support multiple attack infrastructures.
* Although the servers never interact with the target, they can be associated with those parts of our attack infrastructures that do.
* Virtual servers (VPS) can be hosted on one or many cloud providers spread across many geographical locations.

## How?

* [Major cloud providers](major-providers.md)  
* [Research anonymous payments](payments.md)
* [Alternative cloud providers](alt-providers.md)






