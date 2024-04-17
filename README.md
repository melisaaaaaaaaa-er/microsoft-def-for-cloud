# Enable Microsoft Defender for Cloud

<h2>Purpose</h2>

- Enable and Configure Microsoft Defender for Cloud at the virtual machine (VM) and subscription level.

Make sure your Windows and Linux VMs are powered on before starting this lab.

#
<h3>Enable and Configure Microsoft Defender at the VM Level</h3>

<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/microsoft-def-for-cloud-images/main/1.png"/>

Nagivate to Microsoft Defender for Cloud. In the “Getting started” panel, select the the Log Analytics Workspace (here named “law-cyber-lab-01”).

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/microsoft-def-for-cloud-images/main/2.png"/>

Scroll down to “Environment settings”.

Click “Expand all” (where “Collapse all” is on the screenshot) to view the available options.

Click the “...” at the end of the Log Analytics Workspace row and select “Edit settings”.

<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/microsoft-def-for-cloud-images/main/3.png"/>

In the “Defender plans” panel, enable “Servers” and “SQL servers on machines”.

Click “Save”.

<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/microsoft-def-for-cloud-images/main/4.png"/>

Go to the “Data collection” panel and select “All Events”, then “Save”.

Once Microsoft Defender is enabled, it will automatically install an agent on the VMs that facilitate the logging/monitoring process and forwarding logs to the Log Analytics Workspace.

#
<h3>Enable and Configure Microsoft Defender at the Subscription Level</h3>

<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/microsoft-def-for-cloud-images/main/5.png"/>

Go back to Environment settings and edit settings for the Subscription.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/microsoft-def-for-cloud-images/main/6.png"/>

In the  Defender plans panel, enable:
- Servers
- Databases
- Storage
- Key Vaults

Go to “Settings” in the Servers option.

<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/microsoft-def-for-cloud-images/main/7.png"/>

Select “Edit configuration” for the “Log Analytics agent” option.

<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/microsoft-def-for-cloud-images/main/8.png"/>

Select “Custom workspace” and identify the LAW. Choose “All Events” for the “Security events storage” option. Click “Apply”.

<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/microsoft-def-for-cloud-images/main/9.png"/>

Make sure the “Configuration” column reflects the changes just made and click “Continue”.

<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/microsoft-def-for-cloud-images/main/10.png"/>

Click “Save”.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/microsoft-def-for-cloud-images/main/11.png"/>

In the “Continuous export” panel under “Log Analytics workspace”, make sure “Export enabled” is on and select all options for “Exported data types”.

<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/microsoft-def-for-cloud-images/main/12.png"/>

Scroll down and identify the resource group of your VMs for the “Export configuration”, and your LAW for the “Export target”.

Select “Save”.
