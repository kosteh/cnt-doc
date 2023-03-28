---
layout: default
grand_parent: Restore
parent: Processes
title: Request PLP RTO Access
nav_order: 100
has_children: false
---

# Request access to a PLP RTO \<customer\>  

## Context

DevOps teams are used to request PLP resources through the [PLP Portal](https://portal.plp.kadaster.nl). The authorization model of the PLP platform is based 
on the following key components:
- the *PLP customer*  
A Kadaster Business Service (application) runs on computing resources connected to a *PLP Customer* \<customer\>. 
- the *PLP environment*  
The Kadaster Business Service runs in one or more protected (network) environments: ONT(wikkel) (Development environment)), INT(egration and test environment), 
FTO (Functional Test Environment) and/or PROD(uction environment).
- the *PLP \<customer\>-\<environment\>-adm* role  
2 or 3 DevOps team members are responsible to maintain the set of team members that need the *PLP \<customer\>-\<environment\>-dep role*
- the *PLP \<customer\>-\<environment\>-dep* role  
Gives DevOps teams members authorization to request, view or delete PLP platform resources for a specific *PLP \<customer\>-\<environment\>* combination.

More information about the PLP platform can be found on the [PLP documentation site](https://documentatie.plp.kadaster.nl/).

## RTO environment purpose
The PLP environment RTO (Restore Test Omgeving) is a [new PLP environment](/docs/restore/infrastructure). The purpose of the PLP RTO environment is unfortunately not described on the [PLP documentation site](https://documentatie.plp.kadaster.nl/).

{: .highlight }
The RTO has been designed for a very specific purpose: to test *Point-In-Time restores* of production backups of a Business Service or a chain of Business Services.  

{: .warning }
These backups may contain (privacy) sensitive data. Because of this, the RTO is designated as a *restricted environment*. Only DevOps team members involved in restore tests are allowed to access this environment, to deploy application components, to have backups restored and to test the restore as a whole. The *\<customer\>-rto-adm* role is therefore reserved for [TCS team members](docs/team) only.

## Process


