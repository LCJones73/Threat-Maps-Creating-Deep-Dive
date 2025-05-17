# Threat-Maps-Creating-Deep-Dive
### A deep dive into creating Threat Maps, they're importance and usefulness.

# 🛡️ Threat Map Step-by-Step Guide

Importance and Usefulness of Threat Maps:
1. Ehanced Situational Awareness: Mapping threats to your IT environment allowing you to view potential vulnerabilities and attack vectors.<BR>
2. Integration with MITRE ATT&CK Framework: Microsoft Sentinel integrates with the MITRE ATT&CK® framework, allowing you to map detected threats and analytics rules.<BR>
3. Proactive Threat Hunting: Threat maps support proactive threat hunting by enabling analysts to visualize and explore relationships between different threat indicators and activities.<BR>
---
> [!NOTE]
> This guide assumes you have an existing Resource Group in Microsoft Sentinel. For this tutorial, I'll use "_LAW-Cyber-Range_" as an example.
> 
> If you prefer watching a video tutorial, I created one: "_Link Coming Soon_"

---

## 📍 Azure Threat Map Creation

1. **Log into [Azure Portal](https://portal.azure.com/).**<BR><BR>
2. **Navigate to Microsoft Sentinel.**
   ![Step 2 Sentinel](https://github.com/user-attachments/assets/a6a705d1-5389-4bd0-bc47-f83bc6f61606)<BR><BR>
3. **Select your Resource Group** (e.g., `LAW-Cyber-Range`).
   ![Step 3 LAWCyberRange](https://github.com/user-attachments/assets/3276edc6-0d2b-4353-b1f7-23dd91e40547)<BR><BR>
4. **Click on Workbooks** in the left-hand menu.<BR>
   ![Step 4 Workbooks](https://github.com/user-attachments/assets/b744233d-1074-4035-a64e-edfc2a877d4f)<BR><BR>
6. **Click `+ Add Workbook`.**
    ![image](https://github.com/user-attachments/assets/aed1a8d3-6cab-4bf1-8247-6c9b08d53596)<BR><BR>
7. **In the new workbook, click `Edit`.**
10. **For the two panels on the right:**
   - Click the **ellipsis (`...`)**.
   - Select **Remove**.
11. **Click `+ Add` and choose `Add query`.**
12. **Click on `Advanced Editor`.**
13. **Paste your KQL code into the editor.**
14. **Click `Done Editing` at the bottom left.** Your Threat Map is now created!
15. **To save:**
    - Click the **Disk** icon.
    - Choose **`Save As`** to store your Threat Map with log data results.

---

## 🧠 Breaking Down the KQL Code

1. **With the Threat Map open, click `Edit`.**
2. **Under the map, on the bottom right, click `Edit` again.**
3. **Copy the Log Analytics KQL Code displayed.**
> [!TIP]
>  *(Optional)* **Click on `Map Settings`** to customize map functionalities, such as color schemes and data displays.

---

## 📊 Azure Sentinel Log Analytics

1. **Log into [Azure Portal](https://portal.azure.com/).**
2. **Navigate to Microsoft Sentinel.**
3. **Select your Resource Group** (e.g., `LAW-Cyber-Range`).
4. **Click on `Logs`.**
   - *If the `Queries hub` screen appears, click the `X` at the top right to close it.*
5. **On the right side of the screen:**
   - *If it says `Simple Mode`, click the down arrow and switch to `KQL`.*
   - *You may be prompted to set `KQL Mode` as default. Choose accordingly.*
6. **Paste the KQL code you copied from the Threat Map Workbook.**
7. **Analyze the code to understand its components and functionality.**

---

## 💾 Accessing Saved Threat Maps

1. **Follow steps 1–5 from the [Azure Threat Map Creation](#-azure-threat-map-creation) section to navigate to `Workbooks`.**
2. **Click on `Open`.**
3. **Locate and click on your saved workbook to view the results.**

---
> [!IMPORTANT]
> ### Conclusion: Threat Maps in Microsoft Sentinel are vital for visualizing and understanding the complex landscape of cyber threats within your organization. They enhance situational awareness, integrate with established frameworks like MITRE ATT&CK®, and support proactive threat hunting. By leveraging workbooks, custom mapping, and _"Structured Threat Information Expression"_ (STIX) objects, you can create comprehensive threat maps that inform and strengthen your security posture.
---
