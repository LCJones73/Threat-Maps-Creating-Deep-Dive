# Threat-Maps-Creating-Deep-Dive
### A deep dive into creating Threat Maps, they're importance and usefulness.

# Table of Contents

- [Azure Threat Map Creation](#Azure-Threat-Map-Creation)
- [Breaking Down the KQL Code](#Breaking-Down-the-KQL-Code)
- [Azure Sentinel Log Analytics](#Azure-Sentinel-Log-Analytics)
- [Accessing Saved Threat Maps](#Accessing-Saved-Threat-Maps)

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

## Azure Threat Map Creation

1. **Log into [Azure Portal](https://portal.azure.com/).**<BR><BR>
2. **Navigate to Microsoft Sentinel.**<BR>
   ![Step 2 Sentinel](https://github.com/user-attachments/assets/a6a705d1-5389-4bd0-bc47-f83bc6f61606)<BR><BR>
3. **Select your Resource Group** (e.g., `LAW-Cyber-Range`).<BR>
   ![Step 3 LAWCyberRange](https://github.com/user-attachments/assets/3276edc6-0d2b-4353-b1f7-23dd91e40547)<BR><BR>
4. **Click on Workbooks** in the left-hand menu.<BR>
   ![Step 4 Workbooks](https://github.com/user-attachments/assets/b744233d-1074-4035-a64e-edfc2a877d4f)<BR><BR>
5. **Click `+ Add Workbook`.**<BR>
    ![image](https://github.com/user-attachments/assets/aed1a8d3-6cab-4bf1-8247-6c9b08d53596)<BR><BR>
6. **In the new workbook, click `Edit`.**<BR>
   ![Step 6 Edit](https://github.com/user-attachments/assets/fffc152a-c85a-47b8-9564-df8001c5ff68)<BR><BR>
7. **For the two panels on the right:**
   - Click the **ellipsis (`...`)**.
   - Select **Remove**.<BR>
   ![Step 7 Remove](https://github.com/user-attachments/assets/3c6150eb-3312-400a-9ffe-1d277a03f89b)<BR><BR>
8.    **Click `+ Add` and choose `Add query`.**<BR>
  ![Step 8 Add   Add Query](https://github.com/user-attachments/assets/59d8549c-a6ab-4cb4-b715-aa8071cbc391)<BR><BR>
9. **Click on `Advanced Editor`.**<BR>
    ![Step 9 Advanced Editor](https://github.com/user-attachments/assets/2899f7fd-1210-47e4-97da-a2f5f1847be4)<BR><BR>
10. **Paste your KQL code into the editor.**<BR>
    ![Step 9 5 KQL Code](https://github.com/user-attachments/assets/15f98f99-c95e-42b4-a848-46e0dfcafc72)<BR><BR>
    Full code used below:
    ![image](https://github.com/user-attachments/assets/340053f4-9e99-4184-8b58-8826241d904f)<BR><BR>
11. **Click `Done Editing` at the bottom left.** Your Threat Map is now created!<BR>
    ![Step 11 Done Editing](https://github.com/user-attachments/assets/c9ab3840-8b8a-474c-b72f-9db6df9e9150)<BR><BR>
    ![Step 12 Threat Map](https://github.com/user-attachments/assets/bd41cee1-5072-476e-8641-a4b7b93ec6fa)<BR><BR>
12. **To save:**
    - Click the **Disk** icon.
      ![Step 13 Save As](https://github.com/user-attachments/assets/c9aaddab-ca6e-4ff5-b513-8adc09e40952)<BR><BR>
13. **To save:**
    - Choose **`Save As`** to store your Threat Map with log data results.<BR>
      ![Step 13 5 Save As Menu](https://github.com/user-attachments/assets/7ead0f34-939d-46c9-a042-863276b7cb7f)<BR><BR>
14. Now your Threat Map is saved.
    - Further down are the instructions on how to access saved Threat Maps.


---

## Breaking Down the KQL Code

1. **With the Threat Map open, click `Edit`.**
   ![Step 1 Edit](https://github.com/user-attachments/assets/a0795ac5-c013-4215-93e1-10c314f805a3)<BR><BR>
3. **Under the map, on the bottom right, click `Edit` again.**<BR>
   ![Step 2 Edit](https://github.com/user-attachments/assets/a6afd16c-b81d-417c-b0c8-fbd35327e4fe)<BR><BR>
5. **Copy the Log Analytics KQL Code displayed.**<BR>
   ![Step 3 KQL Code](https://github.com/user-attachments/assets/c2838f53-1b75-4723-bc47-cd97edcdcf2a)<BR><BR>
> [!TIP]
>  *(Optional)* **Click on `Map Settings`** to customize map functionalities, such as color schemes and data displays.
  ![Step 4 Map Settings](https://github.com/user-attachments/assets/eb008a53-6b3b-4c41-87fc-0440954020e3)<BR><BR>


---

## Azure Sentinel Log Analytics

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

## Accessing Saved Threat Maps

1. **Follow steps 1–5 from the [Azure Threat Map Creation](#-azure-threat-map-creation) section to navigate to `Workbooks`.**
2. **Click on `Open`.**<BR>
   ![Step 2 Open](https://github.com/user-attachments/assets/3df122e1-6fab-43df-a69b-e97c28686c7f)<BR><BR>
3. **Locate and click on your saved workbook to view the results.**<BR>
   ![Step 3 Your Saved Workbook](https://github.com/user-attachments/assets/f3c413c8-8b03-46d0-abe3-2bedd513e041)<BR><BR>

---
> [!IMPORTANT]
> ### Conclusion: Threat Maps in Microsoft Sentinel are vital for visualizing and understanding the complex landscape of cyber threats within your organization. They enhance situational awareness, integrate with established frameworks like MITRE ATT&CK®, and support proactive threat hunting. By leveraging workbooks, custom mapping, and _"Structured Threat Information Expression"_ (STIX) objects, you can create comprehensive threat maps that inform and strengthen your security posture.
---
