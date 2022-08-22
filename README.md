User management
===
# Overview
ThreatMark uses HTTP authorization to manage access to the AFS Panel. Different users have different roles and thus can use the system in multiple different ways.
# User Roles Description
Here’s a brief overview of the roles you will encounter in the environment.
| User Role | Rights | Description |
|---|---|---|
| Logged | <ul><li>Can see only users with user role Logged</li><li>Can create other users<br>(Role not present in production)</li></ul> | Base role used as a template for creating other user roles |
| Auditor | <ul><li>Can see all the environment</li><li>Can see rules created by the bank administrators</li><li>Can see what other users exist in the environment</li><li>Can investigate the activity log</li><br><li>Cannot modify, delete, or otherwise change the configuration</li></ul> | TBC |
| Bank Analyst | <ul><li>Can access and modify the dashboards on the landing screen of the AFS Panel</li><li>Can access detections in the Detection overview</li><li>Can look up the clients and their sessions</li><li>Can solve cases in the case management</li><li>Can create, edit and modify the lists of IP Addresses, Accounts and Others in the Lists section</li></ul><br>**From AFS v3.37**<br><ul><li>Can manually create a case in case of management without the use of the rule engine</li></ul> | The users with this role generally belong in the fraud investigation team and work as fraud analysts. |
| Bank Admin | <ul><li>Can access the whole of the environment</li><li>Can create, edit and delete rules in the rule engine</li><li>Can create, edit and delete Lists</li><li>Can create, activate and deactivate users on the environment</li><li>Can create the following roles:</li><ul><li>Logged</li><li>Auditor</li><li>Bank Analyst</li></ul></ul><br><ul><li>Cannot create another Bank Admin<br>(Please reach out to ThreatMark Support with a Service Request in our Jira portal)</li></ul> | Bank Admin is the role with the most privileges a client can have. The users with this role are generally system administrators,owners of applications, or heads of fraud departments. |
| TM Analyst | <ul><li>Can do what Bank Analyst does</li></ul><br>**Additionally:**<ul><li>Can create rules in the rule engine</li><li>Can edit existing bank rules</li><li>Can update and manage the Lists section</li></ul> | TM Analyst is ThreatMark’s equivalent of a Bank analyst. The users with this role generally belong to ThreatMark’s SOC fraud department. |
| TM Admin | <ul><li>Can edit and create roles</li><li>Can edit and create users with all available roles</li><li>Can create, modify, and delete the rules in the rule engine</li><li>Can create, modify, and delete Lists in the List section</li><li>Can deactivate rules</li><li>Can create other Bank Admins</li></ul> | TM Admin is the role with the highest privileges in the environment. Users with this role generally include a PM, Delivery Consultant, and members ofThreatMark's Customer Care department. |
# Creation of a New User
To create user accessing AFS Panel:
1. Login as Bank Admin User Role
2. Navigate to **Settings -> Users** and click the green **Add user** button on the upper left side of the screen.

![](https://i.imgur.com/1LDGE2i.png)

