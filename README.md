# Microsoft Sentinel SIEM Implementation in Azure Cloud

## Objective
The **Microsoft Sentinel SIEM Implementation** project involved deploying a Security Information and Event Management (SIEM) solution in the Azure cloud to enable efficient monitoring, analysis, and response to security events. Through advanced configuration and custom rules, I enhanced the SIEM’s threat detection capabilities, gaining practical experience in investigating and remediating security incidents, and strengthening my cybersecurity problem-solving skills.

### Skills Learned
- **Proficiency in SIEM Configuration and Management**: Set up Microsoft Sentinel for centralized monitoring and response to security threats.
- **Advanced Threat Detection Techniques**: Developed custom analytics using KQL to identify specific attack patterns.
- **Incident Investigation and Analysis**: Used SIEM tools to understand and manage cybersecurity incidents effectively.
- **Remediation and Response Implementation**: Applied techniques to mitigate security risks and prevent lateral movement in compromised accounts.
- **Hands-On Experience with Azure Security**: Configured playbooks, watchlists, and incident investigation tools in Microsoft Sentinel.

### Tools Used
- **Microsoft Sentinel**: SIEM solution for centralized monitoring, detection, and response to security threats.
- **Azure Cloud Platform**: Environment for deploying and managing Sentinel and associated resources.
- **KQL (Kusto Query Language)**: Used to develop custom detection rules and analytics in Microsoft Sentinel.
- **Brave Tor Browser**: Used to simulate threat activity by signing into Azure with anonymous access.

## Steps

### Step 1. Deploy Microsoft Sentinel from GitHub Repository
- Successfully deployed **Microsoft Sentinel** from the official GitHub repository in Azure.
- Configured the SIEM tool for centralized threat monitoring.

**Screenshot 1: Microsoft Sentinel Deployment in Azure**  
**Ref 1:** Screenshot showing the Microsoft Sentinel deployment in Azure.

![image](https://github.com/user-attachments/assets/5ccace50-a4cb-43c0-9ed9-f91f7b5147bd)

### Step 2. Enable Artificial Intelligence in SIEM
- Enabled User and Entitiy behaviour analytics (UEBA) and applied it to existing data sources. 

**Screenshot 2: Enabling UEBA**  
**Ref 2:** Screenshot of UEBA being configured in Microsoft Sentinel.

![image](https://github.com/user-attachments/assets/cfc22581-b895-45fb-a67f-020e69f9df37)

### Step 3. Create a Watchlist to Detect Cybersecurity Threats
- Uploaded a CSV watchlist of known threat IP addresses to help in identifying suspicious activity.
- Configured Sentinel to cross-reference this watchlist during threat detection.

**Screenshot 3: Watchlist Configuration**  
**Ref 3:** Screenshot showing the uploaded watchlist in Microsoft Sentinel.

![image](https://github.com/user-attachments/assets/6f5a8244-e2f4-4ed7-9f68-e5fdf6818fa7)

### Step 4. Create a Detection Rule for Cybersecurity Threats
- Created a KQL detection rule to identify login attempts from IPs associated with the Tor network.
- Configured the rule to exclude invalid usernames and capture detailed information for each successful login from these IPs.

**Screenshot 4: Detection Rule with KQL**  
**Ref 4:** Screenshot of the detection rule setup with KQL query in Microsoft Sentinel.

![image](https://github.com/user-attachments/assets/6e9a1e54-5d9b-4bcc-b6b9-6bf38080a115)

### Step 5. Simulate Suspicious Activity Using a New User Account
- Created a test user account with a **contributor role** to simulate unusual activity.
- Logged in with the test account using the Brave Tor browser to generate incidents in Sentinel.

**Screenshot 5: User Account Activity Simulation**  
**Ref 5:** Screenshot of the test user’s login events recorded in Microsoft Sentinel.

![image](https://github.com/user-attachments/assets/dc30d229-b2ab-4dbd-9627-9ba68cba86c5)

### Step 6. Perform Malicious Actions as an Attacker Simulation
- Changed the test account’s password and deleted diagnostic settings, simulating typical attacker actions.

**Screenshot 6: Simulated Malicious Actions**  
**Ref 6:** Screenshot showing malicious activity such as password change and diagnostic setting deletion.

![image](https://github.com/user-attachments/assets/acbfa5e2-2961-4eb0-9794-2aa9f0a3955e)

### Step 7. Investigate Cybersecurity Incidents in Sentinel
- Signed back into the original admin account to investigate the simulated incident.
- Reviewed new incidents in Microsoft Sentinel, identifying multiple suspicious sign-ins and high-severity alerts.
- Analyzed the login patterns to observe multiple logins from different countries, indicating possible malicious behavior.

**Screenshot 7: Incident Investigation in Sentinel**  
**Ref 7:** Screenshot displaying high-severity incidents and associated details.

![image](https://github.com/user-attachments/assets/e1c026ec-ed45-4ecf-addb-3303c255e2d1)

**Screenshot 8: Incident Analysis - Threat Actor Activity**  
**Ref 8:** Screenshot showing the Threat Actor account logging in from multiple countries within a short timeframe, indicating "impossible travel." This pattern strongly suggests malicious activity.

![image](https://github.com/user-attachments/assets/5036222e-8905-45bd-b6d4-4d868e083a91)

**Screenshot 9: Incident Analysis**  
**Ref 9:** This screenshot shows Microsoft Sentinel's 'Entity Behaviours' feature within the Threat Management section. Providing a detailed view of user activity, helping to identify patterns and behaviors that can be crucial for detecting potential threats.

![image](https://github.com/user-attachments/assets/274a3ffc-14df-49f6-92de-18485c1e4a97)

### Step 9. Conduct Remediation Actions
- Disabled the test user account to prevent further access.
- Enabled diagnostic settings and audit logging to capture all security-relevant activities.

**Screenshot 10: Remediation Actions - Account Disablement**  
**Ref 10:** Screenshot showing the account disablement.

![image](https://github.com/user-attachments/assets/8b5e01f9-319d-430d-b4bf-29ddb998ce2d)

**Screenshot 11: Remediation Actions - Enabling Diagnostic Logs**  
**Ref 11:** Screenshot showing the re-enabled diagnostics.

![image](https://github.com/user-attachments/assets/4fd705ea-b128-4c46-911a-2a7c9e3b22b3)




