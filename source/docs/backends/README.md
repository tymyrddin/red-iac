# Introduction

## What?

In the grove we have been using tools such as Metasploit and Empire for post-exploitation. For red teaming some of 
these tools are still useful, but for others we will have to switch to other tools.

## Why?

* For the best part of the last decades the undefeated champion of C2 frameworks was the Metasploit framework, but the 
default settings of the tool have been flagged by every Windows security product since 2007. For hacking Linux PC's it 
can still be a good choice.
* The Empire framework provides an exhaustive list of modules, exploits, and lateral movement techniques specifically
designed for Active Directory. It is no longer maintained by the original team, and BC Security, released version 3.0 
in December 2019. The framework assumes that PowerShell allows attackers unhindered access to the environment. As of 
Windows 10, with PowerShell block logging and AMSI, this is no longer the case.

## How?

* [About C2s](c2s.md)
* [Metasploit container](metasploit.md) for Linux and macOS targets
* [SilentTrinity container](silenttrinity.md) for Windows targets






