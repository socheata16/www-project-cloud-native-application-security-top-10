CNAS-10: Ineffective logging & monitoring (e.g. runtime activity)
===========================================

## Overview

Logging is the technique of recording faults and changes to assist DevOps teams with problem-solving. It also helps with trend detection, security of sensitive data, and the creation of written records. Monitoring is the process of instrumenting an application to gather, aggregate, and analyze metrics for a more accurate assessment of system usage. Teams should integrate instrumentation and monitoring on all systems.

## Description

In order to give a variety of data points that may be used to track the performance and health of infrastructure, logging and monitoring are two processes that work together. A detailed record of system events is created through logging, which records log events produced by programs, devices, or web servers. Monitoring the performance of an application is improved by an effective logging technique.

For attackers to avoid taking advantage of a flaw in object-level permission in an API, such as getting access to login credentials-changing capability for a different user with higher capabilities, a monitoring and logging system is necessary. These kinds of problems can be caught, and it can even stop attempted attacks. 

## How To Prevent
To avoid improper logging and monitoring, OWASP suggests the following actions:

* All login, access control, and server-side input validation errors should be logged with sufficient user context to identify suspicious or malicious accounts. Logs should be retained for a period of time that allows delayed forensic analysis.
* Ensure that logs are created in a format that can be easily used by central log management tools.
* High-value transactions should have an audit trail with integrity controls to prevent manipulation or deletion.
* Effective monitoring and alerting should be established so that suspicious activities can be detected and responded to in a timely manner.
* A response and recovery plan shall be established for incidents, such as NIST 800–61 rev. 2.
* Backup log files on multiple servers to enable fault tolerance
* Always perform penetration tests to identify gaps in incident monitoring and reporting

## Example Attack Scenarios

### Scenario #1

Tom got an email stated "We get a request to reset the password for your account," In case it's not you, kindly click the link.

If you choose to do this, kindly disregard the email. 

Tom clicked on the link by accident and followed the directions without really paying attention to where the email came from. At that point, the hacker has an excellent opportunity to enter and take his information.  

### Scenario #2

A software bug allowed for the hacking of an open source forum project. The attackers were successful in removing the entire forum as well as the internal source code repository containing the future release. The forum software project is no longer functioning because there was a far worse breach because there was no monitoring, logging, or warning.

## References

* Link: https://owasp.org/Top10/A09_2021-Security_Logging_and_Monitoring_Failures/ 

### External

* Link: https://crashtest-security.com/insufficient-logging-monitoring-guide/ 