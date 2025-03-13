# osTicket-Lifecycle


<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Lifecycle Stages</h2>


First we will open a new ticket as an end user > http://localhost/osTicket > Open a New Ticket > Fill out the information > "Create Ticket" 

![image](https://github.com/user-attachments/assets/0b724e4d-9787-4d16-96ef-a9a07dc0e795)


You can now login as an agent and view the ticket > login url: http://localhost/osTicket/scp/login.php > Go to "Agent Panel" > Tickets > In here you can see the new ticket created 

![image](https://github.com/user-attachments/assets/17e94105-4f15-4f92-8668-afddc3059b4a)

If you cannot see the ticket, that means the ticket has been sent to the wrong department. To troubleshoot this we can login as an admin >   Agent Panel > You should see the ticket here, click on it > Once you have opened the ticket you can see what Department it was sent to, so in my case it was sent to "Maintenance"

![image](https://github.com/user-attachments/assets/01096333-cef9-4a3b-b98e-d399bc3ec053)

If you want to delete the Department, you can go to > Admin Panel > Agents > Departments > Check the box, click on "More" > Delete, For this tutorial I will be deleting the Maintenance Department, as it is not necesarry.

![image](https://github.com/user-attachments/assets/aae25eb8-41d2-499a-9b13-6ec61f910c3d)


Since I deleted the "Maintenance" Department, the ticket has automatically been redirected to the "Support Department" 


![image](https://github.com/user-attachments/assets/4302a621-2df5-4f28-8de4-955c5a5be89c)


Since my agent Mads, does not have access to the Support Department, I will grant him access > log in as admin > go to Admin Panel > Agents > Click on the agent > Access > Extended Access > I will give my agent Mads "all access" to the support department

![image](https://github.com/user-attachments/assets/4b80e3f9-6de8-4f2c-be2a-510f3cba19fc)


<h2>Working Tickets</h2>

Open the ticket, in this case Robert is saying that his employees cannot access online banking. This is a really severe issue, so first we will change the SLA plan from default to Sev-A.


![image](https://github.com/user-attachments/assets/ee205570-ef81-49de-83fb-198882fe3b0c)


Next we can look at is "Help Topic", the end user Robert assigned it as "Report a Problem", which is not incorrect. But it is not very precise either. I will change that, to something more precise > Click on the assigned Help Topic > I will change it to "Business Critical Outage" and leave a note on the ticket.

![image](https://github.com/user-attachments/assets/553ef086-08d6-41a6-ac8e-60037eea9d95)


You can also assign the ticket directly to a specific agent or team. I will be assigning this ticket to the "Online Banking" team. > "Assigned to" > Click on the assignment and update it


![image](https://github.com/user-attachments/assets/a7fb6fc9-cddf-4b48-a549-8e14731ac60c)


Scroll down to the botttom of the ticket. Here you can post a response to the ticket. This is a good thing to do to keep the end user updated.


![image](https://github.com/user-attachments/assets/04ae80cd-5048-4cad-aa91-ac2ba449dcf0)

Once the issue has been solved you can post a response in the tickets thread with the solution. This is a good way to document your work.


![image](https://github.com/user-attachments/assets/5eea5d32-16ce-419f-9ccc-9b08ea659277)


Now that we have fixed the issue, we will set the ticket to "resolved" > Status: -> Open, change to "resolved" > close > and ticket is now resolved. 


![image](https://github.com/user-attachments/assets/103d84e8-cb09-4e93-a9e6-680f0357aa74)


As an admin you can see all the closed/resolved tickets > Agent Panel > Tickets > Closed - Here we can see all the tickets that have been resolved this year. You can click into the ticket for more information such as who closed it, what the issue was ect. 


![image](https://github.com/user-attachments/assets/322bbab7-ab93-4311-8f0d-19cf2fa02898)


This is the end of the osTicket tutorial! 

