<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

# osTicket - Ticket Lifecycle: Intake Through Resolution
This tutorial provides a detailed explanation of the entire process a ticket goes through within the open-source helpdesk ticketing system osTicket, from the moment it is submitted to when it is finally resolved. To start, I will demonstrate how a ticket is created by a user facing a real issue. Then, I will show how an agent accesses the ticketing system to begin the process of resolving the ticket.<br/>

## Environments and Technologies Used

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop (Windows 11)
- Internet Information Services (IIS)

## Operating Systems Used

- Windows 10</b> (22H2)

## Ticket Lifecycle Stages

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

## Lifecycle Stages

### Stage 1. ) Intake - Creating Tickets

The first thing we will do is create a ticket from the user end of the osTicket platform.

- Open osTicket: http://localhost/osTicket/

- Select: `Open a New Ticket`

<p align="center"><img src="https://i.imgur.com/4Slnd3I.png"/></p>


- <ins>Insert the following ticket information</ins>:

  - Email Address: `Karen@osticket.com`

  - Name: `Karen Karen`

  - Help Topic: `Business Critical Outage`

  - Issue Summary: `Entire mobile online banking is down`
 
  - Ticket Details: `Customers are reporting they are getting a 404 error when browsing to online banking.`

  - Click: `Create Ticket`

    <p align="center"><img src="https://i.imgur.com/Hocs7bO.png"/></p>
    
>**Note: *When mobile online banking is down, it can lead to a major loss in revenue for the company.***


***

### Step 2. ) Assignment and Communication

- Login to osTicket as an Agent: `(User: jane.doe / jane.doe@gmail.com)`

<p align="center"><img src="https://i.imgur.com/6ipKM19.png"/></p>



***

- Click: The `entire mobile online banking is down`
  (this is the ticket we just created on the user end as Karen)
 
<p align="center"><img src="https://i.imgur.com/1qsE9NG.png"/></p>

***
For the ticket to be handled properly, information regarding the severity level can be changed.
Because the entire mobile banking is down and critical to business impact, we will change the priority
of this ticket to EMERGENCY and the SLA to SEV-A.

<p align="center"><img src="https://i.imgur.com/Dd8m7IY.png"/></p>

- Priority: `Emergency`

  - Type In: `Business Impacting Event`
 
  - Click: `Update`


***
 We will also transfer the ticket to the system administrators department and then assign it to an agent, who in this case will be ourselves, Jane Doe.

- Click: `Department`

  - Select: `System Administrators`

  - Details: `Sys Admins responsible for mobile banking infrastructure`
 
  - Click: `Transfer`

<p align="center">
<img width="800" alt="isolated" src="https://i.imgur.com/Hw2VHyq.png"><br></p>

***

- Assigned to: `Jane Doe`

  - Click: `Assign`

<p align="center">
<img width="800" alt="isolated" src="https://i.imgur.com/WaMBNU3.png"><br>

***

- SLA Plan: `SEV-A`

  - Details: `Business Impacting, Critical Event`
 
  - Click: `Update`

<p align="center">
<img width="800" alt="isolated" src="https://i.imgur.com/Dd8m7IY.png"><br>

***

>**Note: *Make sure your ticket information matches the image below and continue to the next step.***

<p align="center">
<img width="800" alt="isolated" src="https://i.imgur.com/N2HuQJg.png"><br>

***

>**Note: *This is where you will see the history and updates of the tickets. &darr;***

<p align="center">
<img width="800" alt="isolated" src="https://i.imgur.com/UOOBCD6.png"><br>

***

### Stage 3. ) Working the Issue

- On the back end, Jane is working with the System Adminstrator team to resolve the issue.

- Response Text Box: `Coordinating with Sys Admin Team to bring mobile banking back online.`

- Select: `Post Reply`


<p align="center">
<img width="800" alt="isolated" src="https://i.imgur.com/ABuZ4RN.png"><br>
**Note: *The organization you work for will determine the type of details you type into the description.**


***

### Stage 4. ) Resolution
     
- Return to the ticket and update the end user once the issue is resolved.

- Response Text Box: `Jerry from System Engineering found and connected a failed load balancer. Mobile banking should be back up.`

- Ticket Status: `Resolved`

- Select: `Post Reply`

<p align="center">
<img width="800" alt="isolated" src="https://i.imgur.com/Ld8YOkj.png"><br>

***

*<ins>The ticket should now be on the "closed" tab since it has been resolved.</ins>*

<p align="center">
<img width="800" alt="isolated" src="https://i.imgur.com/G4uqKcr.png"><br>

 Congratulations! You have successfully resolved your first ticket as a help desk support agent! 
