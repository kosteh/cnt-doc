---
layout: default
grand_parent: Restore
parent: Processes
title: Request PLP RTO Authorization
nav_order: 100
has_children: false
---

# Request PLP RTO Authorization

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

## Purpose of the RTO environment
The PLP environment RTO (Restore Test Omgeving) is a [new PLP environment](/docs/restore/infrastructure). The purpose of this environment is unfortunately not described on the [PLP documentation site](https://documentatie.plp.kadaster.nl/).

{: .note }
The RTO has been designed for a very specific purpose: to test *Point-In-Time restores* of production backups of a Business Service or a chain of Business Services.  

{: .warning }
These backups may contain (privacy) sensitive data. Because of this, the RTO is designated as a *restricted environment*. Only DevOps team members involved in restore tests are allowed to access this environment, to deploy application components, to have backups restored and to test the restore as a whole. The *\<customer\>-rto-adm* role is therefore reserved for [TCS team members](/docs/team) only.

# Request RTO authorization
Ask the product owner (PO) responsible for the Business Service \<customer\> to:
1. Create an e-mail for [continuiteit@kadaster.nl](mailto:continuiteit@kadaster.nl)
2. Subject: PLP-RTO deployment role authorization request
3. The body of the mail should contain the following information:  
  -- Customer: *the name of the PLP customer for which the RTO deployment role is requested*  
  -- Name: *the full name of the DevOps team member that needs the RTO deployment role*  
  -- Accountname: *the AD short accountname*  
4. Send the mail.

The TCS team will execute your request as soon as possible and will send a an e-mail reply as soon as possible to the requester (the Product Owner) and the DevOps team member it concerns.






LTB desk





Business Service 
PO
Herstelplan link


Restricted for deployment is 1
Applicatie gebruik (https:// appl toegang)
