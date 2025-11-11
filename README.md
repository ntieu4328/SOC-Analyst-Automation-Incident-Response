<h1>SOC Analyst Automation Setup</h1>

<h2>Description:</h2>

After completing the [SOC Analyst Automation setup](https://github.com/ntieu4328/SOC-Analyst-Automation-Setup), I will now simulate what an incident response situation would look like. You can simulate different incidents that will show up in TheHive or Wazuh. The incident that I will be simulating will be failed login attempts.

<h2>Environments Used:</h2>

   - Wazuh
   - TheHive
   - Windows 10

<h2>Walk-through:</h2>

<h3>Create Incident:</h3>

1. Log out of the account to get to the Windows 10 login screen:

![windows 10 login](https://github.com/ntieu4328/SOC-Analyst-Automation-Incident-Response/assets/156137990/fac132d8-dcb3-44fa-83e5-38cb336ddb9e)

2. Continuously log in with incorrect information.

3. The failed login information should show in both Wazuh and TheHive:

Wazuh:

![Windows Logon Failure alert wazuh](https://github.com/ntieu4328/SOC-Analyst-Automation-Incident-Response/assets/156137990/7fb90aa3-3ba4-42f8-92f0-89562e1bfd92)

TheHive:

![Windows Logon Failure alert TheHive](https://github.com/ntieu4328/SOC-Analyst-Automation-Incident-Response/assets/156137990/bcecb209-4863-46bb-b47e-fa9dad41d552)

![Inside Logon Failure Alert](https://github.com/ntieu4328/SOC-Analyst-Automation-Incident-Response/assets/156137990/f7efc341-c428-4876-861c-b22eb7446238)
<br>
<br>


<h3>Incident Response:</h3>

If I was in an organization and I wanted to respond to this incident I would forward this to an analyst. I made a user on TheHive who will act as a fake Analyst in my organization.

1. Create case:

  - You can change the information in the Description to make it more clear
  - You can change the severity of the incident
  - <b>IMPORTANT</b> You can create a task that you can forward to users or analysts in the organization

![create case](https://github.com/ntieu4328/SOC-Analyst-Automation-Incident-Response/assets/156137990/c04e058c-7173-4734-a9c1-2682686056ff)

2. Create Task:

![add task](https://github.com/ntieu4328/SOC-Analyst-Automation-Incident-Response/assets/156137990/1b72a2d6-eb1c-4044-9be7-eb2c2763a9c5)

3. Recieve and act on task:
*I logged into the TheHive account that I made that should receive the task

![task received](https://github.com/ntieu4328/SOC-Analyst-Automation-Incident-Response/assets/156137990/c923c2b0-d4ec-4437-85d5-2c6e6f67b25c)

The analyst or user that receives the task can now act on it.

<b>Finished responding to the incident!!!</b>
