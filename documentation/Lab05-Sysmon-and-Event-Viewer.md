Sysmon & Windows Event Viewer

Objective

Install Sysmon and use Windows Event Viewer to monitor and investigate system activity generated on a Windows Server 2022 Domain Controller.

---

Environment

* Windows Server 2022 (Domain Controller)
* Windows 11 Domain Client
* Kali Linux
* Oracle VirtualBox

---

Tasks Performed

* Downloaded Sysmon from Microsoft Sysinternals
* Installed Sysmon on the Domain Controller
* Applied the SwiftOnSecurity Sysmon configuration
* Verified the Sysmon service was running
* Opened the Sysmon Operational log in Event Viewer
* Generated activity using Command Prompt and PowerShell
* Investigated Sysmon events

---

Events Investigated

Event ID 1

**Process Creation**

Observed:

* Executable image
* User account
* Parent process
* Command line

---

Event ID 11

**File Creation**

Observed PowerShell creating temporary script policy files.

Learned that not every file creation event indicates malicious activity.

---

Event ID 22

**DNS Query**

Observed Windows services performing DNS lookups under the `NETWORK SERVICE` account.

Learned that Windows background services often generate events independently of the interactive user.

---

Challenges

* Sysmon executable was not initially found because the command was executed from the wrong directory.
* Confirmed Sysmon installation and updated it with the SwiftOnSecurity configuration.
* Investigated why certain expected network events were not immediately visible and learned that event collection depends on the active Sysmon configuration.

---

Lessons Learned

* Sysmon significantly increases Windows logging visibility.
* Event Viewer is essential for investigating Windows activity.
* Security monitoring requires understanding normal operating system behavior before identifying suspicious activity.
* Multiple related events provide better context than analyzing a single event in isolation.

---

Skills Demonstrated

* Windows Server Administration
* Sysmon
* Windows Event Viewer
* Event Analysis
* PowerShell
* Troubleshooting
* Security Monitoring
