---
layout: default
parent: Processes
title: Request PLP RTO Access
nav_order: 100
has_children: false
---

# Request access to a PLP RTO \<customer\>  

## Introduction to the PLP Portal

DevOps teams are used to request PLP resources through the [PLP Portal](https://portal.plp.kadaster.nl). The authorization model of the PLP platform is based 
on the following key components:
- the *PLP customer*  
A Kadaster Business Service (application) runs on computing resources connected to a *PLP Customer* \<customer\>. 
- the *PLP environment*  
The Kadaster Business Service runs in a protected (network) environment: ONT(wikkel (Development environment)), INT(egration and test), 
FTO (Functional Test Environment) and PROD(uction).
- the *PLP \<customer\>-\<environment\>-adm* role  
2 or 3 DevOps team members are responsible to maintain the set of team members that need the *PLP \<customer\>-\<environment\>-dep role*
- the *PLP \<customer\>-\<environment\>-dep* role  
Gives DevOps teams members authorization to request, view or delete PLP platform resources for a specific *PLP \<customer\>-\<environment\>* combination.

More information about the PLP platform can be found on the [PLP documentation site](https://documentatie.plp.kadaster.nl/).

## The RTO environment
The PLP environment RTO (Restore Test Omgeving) is a [new PLP environment](/docs/restore/infrastructure).

{: .highlight }
The RTO has a specific purpose: to test Point-In-Time restores of production backup of a Business Service or a chain of Business Services. These backups may contain (privacy) sensitive data.

Because of that 
