# Threat-Maps-Creating-Deep-Dive
### A deep dive into creating Threat Maps, they're importance and usefulness.

# 🛡️ Threat Map Step-by-Step Guide

> [!NOTE]
> This guide assumes you have an existing Resource Group in Microsoft Sentinel. For this tutorial, I'll use "_LAW-Cyber-Range_" as an example.
> 
> If you prefer watching a video tutorial, I created one: "_Link Coming Soon_"

---

## 📍 Azure Threat Map Creation

1. **Log into [Azure Portal](https://portal.azure.com/).**
2. **Navigate to Microsoft Sentinel.**
3. **Select your Resource Group** (e.g., `LAW-Cyber-Range`).
4. **Click on Workbooks** in the left-hand menu.
5. **Click `+ Add Workbook`.**
6. **In the new workbook, click `Edit`.**
7. **For the two panels on the right:**
   - Click the **ellipsis (`...`)**.
   - Select **Remove**.
8. **Click `+ Add` and choose `Add query`.**
9. **Click on `Advanced Editor`.**
10. **Paste your KQL code into the editor.**
11. **Click `Done Editing` at the bottom left.** Your Threat Map is now created!
12. **To save:**
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
