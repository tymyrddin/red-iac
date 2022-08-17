# Introduction

## What?

The attack infrastructure frontend interacts with the target.

## Why?

* The frontend initiates connections to the target, scans machines, and routes incoming packets from a reverse 
shell through a web proxy to deliver them to a backend systems, a C2 framework like Metasploit or SilentTrinity.
* This packet routing can be done with a regular web proxy like Nginx or Apache that acts as a filter: requests from 
infected computers are routed to the corresponding backend C2, while the remaining requests are displayed an innocent
web page.
* It must be unique to each operation or target, and be quickly replacable every few days.

## How?

* The [Nginx web server](nginx.md) can be tuned relatively quickly.
* [IP masquerading](masquerading.md)





