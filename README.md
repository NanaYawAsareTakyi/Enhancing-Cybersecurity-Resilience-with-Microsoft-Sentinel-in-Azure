# Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure
Enhanced cybersecurity by deploying Microsoft Sentinel in Azure, using advanced threat detection and custom analytics to strengthen defense mechanisms. 

## Objective
This project aimed to enhance cybersecurity resilience by deploying Microsoft Sentinel in Azure. This involved configuring advanced threat detection and custom analytics rules to enable proactive monitoring and rapid response to incidents.

## Skills Learned
#### SIEM Implementation:
Skills in deploying and configuring a Security Information and Event Management (SIEM) solution like Microsoft Sentinel.

#### Advanced Configuration:
Ability to implement advanced configurations within Microsoft Sentinel to optimize threat detection and response.

#### Kusto Query Language (KQL): 
Proficiency in using KQL to create custom analytics rules and queries for specific security events and patterns.

#### Incident Response:
Skills in conducting thorough incident investigations using SIEM tools and techniques, and implementing remediation actions to mitigate and resolve cybersecurity incidents.

#### Cloud Security:
Understanding of cloud security principles and practices, particularly in the context of Azure Cloud and SIEM solutions.

#### Cyber Threat Detection:
Enhanced capability in detecting and analyzing cybersecurity threats, leveraging SIEM capabilities and analytics.

#### Cybersecurity Best Practices: 
Knowledge of best practices for enhancing organizational cybersecurity resilience through effective use of SIEM tools and cloud platforms.

## Tools Used
<img src="https://img.shields.io/badge/-Microsoft%20Sentinel-0078D7?style=for-the-badge&logo=Microsoft%20Sentinel&logoColor=white" /> Security Information and Event Management (SIEM) solution.

<img src="https://img.shields.io/badge/-Microsoft%20Azure-0089D6?style=for-the-badge&logo=Microsoft%20Azure&logoColor=white" /> Cloud platform for hosting and managing Microsoft Sentinel.

<img src="https://img.shields.io/badge/-KQL-4B8BBE?style=for-the-badge&logo=KQL&logoColor=white" /> Used for creating custom analytics rules and querying data within Microsoft Sentinel.

<img src="https://img.shields.io/badge/-Azure%20Portal-0078D7?style=for-the-badge&logo=Microsoft%20Azure&logoColor=white" /> Interface for managing and configuring resources in Azure, including Microsoft Sentinel.

<img src="https://img.shields.io/badge/-CloudShell-0078D7?style=for-the-badge&logo=Microsoft%20Azure&logoColor=white" /> Tool for managing cloud resources and performing cloud-related tasks directly from a web browser.

## Workflow
To expedite the deployment of Microsoft Sentinel, I utilized the official Microsoft solution called "Sentinel All in One", available on GitHub. This resource streamlines the initial configuration tasks effectively and installs some content hub solutions. 

Content hub solutions are pre-configured packages of analytics, rules, dashboards, automation tasks and many more artifacts related to Microsoft Sentinel. This solution also enables data connectors from a list of sources such as Azure Active Directory 365 Defender and threat intelligence platforms allowing users to start ingesting data from different sources immediately.


To start with, I clicked on the “Deploy to Azure” icon on the repository page.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/13436efd-db23-4f42-b452-0920cb5d615d)


This redirects to the Azure portal where I can deploy Microsoft Sentinel from a predefined template. 

On the custom deployment page, I filled in the form with appropriate details like location, resource group, pricing and workspace name.

A resource group is a logical container used to group Azure resources such as virtual machines, databases, web apps, storage accounts and many more. This allows for the collective management of resources with respect to deployment, tagging and security.

The image below illustrates this step:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/3308691b-32a3-487c-bfd5-30d5622cf759)

On the next page, “Settings”. I enabled Sentinel health diagnostics as this would enhance the reliability, performance, and security effectiveness of Microsoft Sentinel within the Azure environment.

This is illustrated in the image below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/74ce88d0-edc3-4c6a-b51d-e435a270045d)

Next, I navigated to “Content Hub Solutions” where I selected all the options in the dropdown menus of the three (3) categories on the page.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/c3471487-55cb-40b6-b22c-ec990ae0c742)

I moved to the “Data Connectors” page where I selected all the options in the dropdown menus of the two (2) categories on the page.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/6cfa7036-85ea-423a-8ad4-8a96c0d6f445)

Next up was “Analytics Rules”, I checked the box to “Enable Scheduled alert rules for selected Content Hub solutions and Data Connectors”. This prompted a dropdown option which allowed me to “Select the severity of the rules to enable”, I ticked the “Select all” box for this.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/991ec84b-a4d2-482d-953b-7d31425a7a9d)

Finally, I reviewed the settings I had made and created my custom deployment for Microsoft Sentinel.

The image below illustrates this:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/9a016cdc-2cc4-47e7-89ef-dd89497d443d)

At this stage, Microsoft Sentinel was successfully deployed. However, I encountered an error related to data connectors that required a license. This should not hinder progress as everything else is set up successfully.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/d7af8d00-0346-4821-aabf-c1650efe42cc)

Next, I selected my resource group. In the resource group a myriad of templates were created to match the analytics rules, a separate template for each rule.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/4fd84290-dad7-4b6a-a067-5b9b375146c0)

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/838e1bee-4197-403d-9616-aea532569062)

I navigated to the log analytics workspace and selected “Diagnostic settings”.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/5479db9f-46a9-448f-8fbe-b5fcd0d54341)

Here I added a new diagnostic setting. I named it appropriately, ticked the boxes for “allLogs”, “AllMetrics” and specified the destination by ticking the “Send to Log Analytics workspace” box. I confirmed the Log Analytics workspace and saved the settings I had made.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/b177b6b0-0905-4b82-b4ca-512b3a3cbcc4)

Next, I navigated back to Sentinel. I simply searched for it in the search bar and selected my deployment. This landed me in the overview section. 

The image below illustrates this:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/b3a11c3a-588f-44b7-85c4-98375c99e3ef)

Next, I navigated to “Settings” under “Configuration” to enable User and Entity Behavior Analytics. I selected Azure Active Directory and applied this setting to existing data sources.

User and Entity Behavior Analytics (UEBA) is a security analytics approach that focuses on monitoring and analyzing the behavior of users and entities such as devices, applications, and services within an IT environment. The goal of UEBA is to detect anomalies, threats, and suspicious activities based on deviations from normal behavior patterns.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/93253c11-e617-48d7-a90e-23ed2c4bdae7)

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/00e240e8-857c-4e55-9f80-6da83aa17869)

I then configured Sentinel to use automation playbooks. To do this, I had to provide Sentinel with the appropriate permissions. I selected “Playbook permissions” on the “Settings” page and clicked on “Configure permissions”. I then selected my resource group where Microsoft Sentinel was deployed and clicked “Apply”.

Playbooks are automated workflows designed to respond to security incidents and alerts. They automate the response to security incidents, significantly reducing the time to react and mitigate threats.

The image below illustrates this:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/a007ab14-8d01-470f-bd9f-76c1a00349c1)

Next, I configured Microsoft Sentinel to monitor Tor exit nodes. This involved setting up Sentinel to detect and analyze traffic originating from Tor exit nodes, which are commonly used for anonymous internet activity and can be exploited for malicious purposes. By closely monitoring these nodes, potential threats, suspicious activities, and security incidents associated with Tor network usage can be identified, enabling proactive threat detection and response.

To accomplish this, I created a watchlist that checks all the Tor exit nodes in IP addresses.

I navigated to the “Watchlist” section under “Configuration” and clicked on “Add new”. Under the “General” section on the Watchlist wizard page, I named my watchlist and provided an alias as well. In the “Source” section I selected “Local file” for “Source type” as I already had a CSV file with all the Tor IP addresses. I uploaded the file on the page and finally selected a unique “SearchKey” to optimize query performance. I then reviewed and created my Watchlist.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/1c001785-2901-4175-8caf-32a8a1f72a22)

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/de15f389-eccd-48cb-9635-5b6f374c5072)

Next, I proceeded to create an analytics rule that would detect threats from Tor network. To add a new analytics rule to Microsoft Sentinel, I navigated to the configuration section and selected “Analytics”. Under “General” in the analytics section, I named the rule appropriately, gave it a befitting description and selected the severity level.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/fbd2489d-5741-4d57-a344-1e12fba56add)

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/582c4c5a-03f7-4247-9ec3-0b0187d1d2c2)

Under “Set rule logic” I used KQL to inform Sentinel on what to look for in data.

To begin the query, I called the watchlist function to retrieve a list of IP addresses and save it as a variable.
I used the command “let TorNodes = (_GetWatchlist(‘Tor-IP-Addresses’) | project TorIP = IpAddress:”.

Next, I specified the table Sentinel should use to look for data. 
I used “SigninLogs” which contains all the signing events for this rule. I used the command “SigninLogs where IPAddress in (TorNodes)”. To reduce the amount of irrelevant data returned, I filtered out for columns I found pertinent.

The KQL query "let TorNodes = (_GetWatchlist('Tor-IP-Addresses') | project TorIP = IpAddress:" defines a variable TorNodes that retrieves and stores IP addresses from a watchlist named 'Tor-IP-Addresses'.
This variable can then be used in further analysis within Microsoft Sentinel for monitoring and analyzing Tor exit nodes.

"let" is a keyword in KQL used to define a variable.

"TorNodes" is the name of the variable being defined. This variable will store the result of the query.

"_GetWatchlist" is a function used to retrieve a watchlist named 'Tor-IP-Addresses'.

Watchlists in Microsoft Sentinel are collections of entities such as IP addresses that are monitored for specific characteristics, in this case, Tor exit nodes.

"|" (pipe), is used to chain operations in KQL.

"project" is used to select specific columns or properties from the dataset.

"TorIP = IpAddress" specifies that we are selecting the IpAddress field from the watchlist data and renaming it as TorIP in the result set.


 My final query is illustrated in the image below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/45e52e69-9af1-4b7c-bf60-c705718de791)

Next, I navigated to the “Entity mapping” section under “Alert enrichment”. 

Entities in Microsoft Sentinel are objects that represent important information about the environment such as hosts, users, IP addresses and many more.

I added two (2) different entities, “Account” and “IP Address”. 

For “Account”, I selected “Account” as entity type, “Sid” as identifier and “UserId” as its corresponding value.
I also added a “DisplayName” with a corresponding value of “UserDisplayName” by clicking on “Add identifier”.

For “IP Address”, I selected “IP” as entity type, “Address” as identifier and “IP Address” as its corresponding value.

Next, I navigated to “Custom details” which allows a user to surface particular event parameters and their values in alerts that comprise those events.

To surface event parameters and their values in alerts that comprise those events means to extract, display, and highlight specific details or attributes of security events within the alerts generated by Sentinel. This involves making key pieces of information from the raw event data visible and accessible in the alert to provide context and enable faster analysis and response.  

I entered key-value pairs of my choosing which will appear as the field name with corresponding values in alerts.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/fe4463e9-5277-484e-acde-418a6d74978a)

Next, I navigated to “Alert details” where I filled in the slots under the section including “Alert Name Format”, “Alert Description Format”, “Alert property” and “Value”.

Finally, I provided my preferred query scheduling parameters under the “Query scheduling” section. This regulates how often the query will run and how far in the past the query will look.

The image below illustrates this:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/b634e698-9cab-4fe1-9ed1-455f08e191ac)

Next, I moved to the “Incident settings” section where I set how the alerts triggered by the analytics rule are grouped into incidents. I grouped all alerts with matching IP addresses and usernames into the same incident.

The image below illustrates this:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/066519ae-b9a6-4d8a-9b0f-cc5c6cacce58)

Finally, I reviewed and created my analytics rule.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/ef0dd575-8557-4881-b219-926b6539abf2)


![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/cfa39e21-3fae-42f5-b00e-680b7468768e)

The next line of action was to create a new account that would perform some unusual activity. 

Before that, I turned off security defaults in the Active Directory to avoid any potential interruption. 

Microsoft automatically turns this feature on for a new Azure Active Directory as it provides a crucial baseline level of protection for all users and accounts in an organization. This includes Multi-Factor Authentication (MFA) for all administrators blocking legacy authentications such as iMap or SMTP which helps to reduce risk of attacks like password spraying and brute force attacks.

To turn this feature off I navigated to “Properties” under Active Directory and clicked on “Manage security defaults”. In the pop-up window on the right, I disabled the default setting. I provided my “Reason for disabling” as “Other” and described it as “testing”. I finally saved the changes I had made.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/a606a5be-e316-401b-a71a-af95c8c24a5f)

I proceeded to create a new account to simulate the actions of a malicious actor..

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/0b2deb90-bf59-4d4a-a2da-3709a132486f)

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/a0c16f66-2d5f-4bfe-8020-e1993dafa925)

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/1376e49f-b138-4754-8412-5555e72aace7)

Next, I assigned some roles to the newly created account.

I clicked on the account name and navigated to “Assigned roles” under the “Manage” section. 

Next, I clicked on “Add assignments” and searched for “Security Reader” and clicked “Assign”.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/8d595b95-807a-4239-b7e7-6dd86180862f)

Next, I navigated to “Access control (IAM)” in the “Resource group” and added a role assignment.

I keyed in the necessary details and then clicked on “Review + assign” to assign the role to the new user account.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/ba881903-92ea-416f-a47c-1ffcfb162ddf)

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/5296a5dc-4eae-4fe2-819e-243bef32136f)

Next, I put my hacker hat on and logged in to the newly created account from Tor network.

I used the Brave browser to accomplish this as it provides the option to create a new window with Tor.

The image below illustrates this:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/0548ac3e-4e3e-42d9-8678-e2e7127efe8f)

As an attacker, my initial step was to establish persistence, which involved changing the password.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/77651797-c285-4adf-b7a2-34fdf759940c)

Next, I disabled and created some resources to provide me with something to work with later.

I navigated to “Diagnostic settings” in the resource group and deleted the diagnostic settings.  

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/2431c561-bac2-4c93-b6c5-19fa53952f2a)

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/ac0c9db2-c162-4d5e-b18d-560eea5ccd40)

Next, I created a virtual machine to demonstrate other malicious actions an attacker could perform.

To replicate real-world attacker behavior, I used generic data to obscure details during the virtual machine creation process.

Thus, I named the VM “Dev-Temporary-VM”. 

After successfully creating the VM, I ran CloudShell as an attacker.

I simply did this by clicking on the CloudShell icon next to the search bar and selecting PowerShell.

CloudShell is an integrated command-line interface (CLI) provided by cloud platforms like Microsoft Azure. It allows users to manage cloud resources directly from their web browser without the need to install any software or configure a local environment.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/1f5bd4f7-f537-4b7d-a5df-a8966a7cfc63)

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/60185f66-953c-4d0c-bbde-e7595b3380f5)

Returning to Microsoft Sentinel, I switched to investigation mode and prepared to examine the situation. 

On the dashboard, several new incidents had been reported.

The image below illustrates this:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/b6f6bf61-36c8-4833-81f6-5eb191a50089)

Under “Threat management”, I clicked on “Incidents”. This directed me to the incident table containing a comprehensive list of all detected incidents.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/ddc60172-1075-48db-acad-7d81c346e46d)

To investigate the incidents of interest at the same time, I clicked on the boxes next to their severity ranking and selected “Actions”. In the pop-up window on the right, I filled in the slots for “Owner” and “Status”. I assigned the incidents to myself, changed their statuses to active and clicked “Apply”. 

This is very essential especially in a Security Operations Center (SOC) team as it establishes accountability. This clarifies responsibility for resolving the incident, ensuring all team members are aware of who is managing it.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/877974e9-b485-43f0-b774-255d741b599c)

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/5ea43ff6-842d-45cd-8aac-473887e19b91)

Next, I selected an incident and viewed its details. This provided a summary of the incident including information about the entities involved such as the username and IP address related to the incident. Access to evidence including events, alerts and bookmarks is also provided.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/b65e2cb1-c0a2-4a69-9e56-2731c0c2aea7)

Clicking on any of these entities reveals additional details.

Clicking on “Events” pops out a new window on the right presenting more details of the incident including authentication method, IP address and origin.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/7e84c7e5-8d88-4d27-b091-0e5033cc42da)

I copied the IP address and checked if it was related to any malicious activity. To do this, I used the freely available service AbuseIPDB.

AbuseIPDB is an online database that tracks reports of malicious activity associated with IP addresses. It serves as a valuable resource for network administrators, security professionals, and anyone involved in cybersecurity to identify and respond to potentially harmful IP addresses.

AbuseIPDB confirmed that the IP address was related to Tor exit nodes. Scrolling down on the page revealed multiple reports of the IP address. This confirmed that the IP address in the incident is truly malicious.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/594a6be8-ec1c-4111-ad91-b0ca54383cd4)

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/cffd6e7b-942d-479e-bfa3-c96032f80423)

I included the “UserPrincipleName” in my next query. To do this I right clicked on “UserPrincipleName” and selected the option to include it.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/a98780d0-d26d-4d2a-9379-99bed9f17a54)

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/132fbce1-8f25-49b5-b436-637a37cd895c)

Next, I removed every other line except for “Signinlogs”, specified the time range for the query, applied changes and ran the query. This provided the sign in history for the specified time range.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/2c1a0f5f-44b4-4a0c-845d-feae25f1177d)

Scrolling to the right reveals the location information of the user. 

The image below illustrates this:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/ace5a237-2436-4896-b7dc-c68ed773765c)

Next, I navigated to “Entity behavior” under the “Threat management” section of the Microsoft Sentinel page. This presented me with the option to search and select the user.

By doing this, I could see all the user activities in one place. This helps to identify any pattern or anomaly that could be relevant to the investigation.

The image below illustrates this:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/244a1aac-b218-4220-adf1-c506d35c552b)

By selecting “ThreatActor”, a new window pops up and displays a graph with all relevant alerts, anomalies and activities. 

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/a7504be5-67a8-4760-afac-1b1a85111814)

Next, I took quick and effective actions to secure the Azure environment from potential threats. 

Firstly, I disabled the compromised account to prevent any further damage.

To do this I navigated to the Active Directory and selected “Users”. I selected the malicious account and disabled the account the status. I did this by simply clicking on “Edit” under the account status, unchecking the “Account enabled” box and saving the change made.

The image below illustrates this:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/ea241405-cacf-4676-8379-f597a76afffa)

Another area of concern was the virtual machine hosted in the Azure environment. To remediate this, I navigated to “Virtual machines”, selected the VM and deleted it.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/28ad79ed-f993-4b93-87ac-ab7a210ad230)

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/dd806bc9-1a9f-458f-a7e4-fc5d6786d3c5)

To further secure the environment, I turned on the diagnostic settings for Log Analytics and Microsoft Sentinel.

To do this I navigated to the Log Analytics workspace, selected my instance and in diagnostic settings I clicked “Add diagnostic setting”. I then enabled “allLogs”, filled out the name, set the destination as the Log Analytics workspace for Sentinel and saved the changes.

From the Sentinel dashboard I moved to “Settings” and enabled auditing and health monitoring.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/efb6429f-085f-48f2-8856-7ff45a34c7d1)

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/ee2bc1dd-ae59-45fc-a2e4-24f4c4b8faee)

After remediating all the issues, I moved to the incident page and closed all the incidents I had assigned to myself. To do this I selected the incidents, clicked on “Actions”, changed the status to “Closed”, selected a “Classification reason”, provided comments and clicked “Apply”.

This is illustrated below:

![image](https://github.com/NanaYawAsareTakyi/Enhancing-Cybersecurity-Resilience-with-Microsoft-Sentinel-in-Azure/assets/173400465/87ad808a-b447-4075-a58e-2e68c6dee3fb)

## Summary
In this project, I successfully deployed Microsoft Sentinel in Azure cloud, transforming the organization's cybersecurity operations. By leveraging advanced configurations and custom KQL rules, the SIEM solution enabled precise detection of security events and patterns. Incident investigations were conducted efficiently, utilizing SIEM tools to analyze and respond to cybersecurity incidents promptly. As a result, the organization enhanced its ability to mitigate and resolve security threats, significantly bolstering its overall cybersecurity resilience.
