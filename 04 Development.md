# Lesson 3: Development – Building & Automating the Solution

In this lesson, we will turn your **To-Be process design** into a **working automation** using the Microsoft Power Platform.

---

## 🎯 Learning Objectives
By the end of this lesson, you will:
- Understand which **Power Platform tool** to use for different tasks
- Build a simple **automation** in Power Automate
- Test and refine your solution
- Share your automation with others

---

## 🛠 Choosing the Right Power Platform Tool

| Task | Tool |
|------|------|
| Collecting information from users | **Power Apps** |
| Automating workflows and actions | **Power Automate** |
| Visualising data and reports | **Power BI** |
| Building chatbots for FAQs | **Power Virtual Agents** |

---

## 🚀 Our First Automation
We will automate part of our **To-Be process**:

**Example scenario:**
When a new entry is added to a SharePoint list, send an automated email to the manager.

---

## 🗂 Step 1: Prepare Your Data
We’ll use **SharePoint** as our data source.

1. Go to [https://office.com](https://office.com) and log in with your Microsoft 365 account.
2. Open **SharePoint** and create a new site (or use an existing one).
3. Create a **List** with the following columns:
   - **Title** – short text (e.g., Request Title)
   - **Description** – multiple lines of text
   - **Requester Email** – single line of text

---

## ⚡ Step 2: Create an Automation in Power Automate

1. Go to [https://make.powerautomate.com](https://make.powerautomate.com)
2. Select **Create** → **Automated cloud flow**
3. Name your flow: `Notify Manager of New Request`
4. Choose trigger: **When an item is created** (SharePoint)
5. Configure the trigger:
   - **Site Address**: Your SharePoint site
   - **List Name**: Your list from Step 1
6. Add an action: **Send an email (V2)**
   - **To**: Manager's email
   - **Subject**: `New request: @{Title}`
   - **Body**: Include `Description` and `Requester Email` from the list
7. Save your flow.

---

## 🧪 Step 3: Test the Automation
1. Go to your SharePoint list.
2. Add a new item (fill in Title, Description, Requester Email).
3. Check the manager’s inbox for the automated email.

---

## 🔁 Step 4: Refine & Improve
- Add conditions (e.g., only email if request is urgent).
- Add approvals (Power Automate has a built-in **Start and wait for an approval** action).
- Integrate with Teams to send notifications directly.

---

## 📌 Activity
1. Take your **To-Be process** from Lesson 2.
2. Identify at least **one step** you can automate in Power Automate.
3. Build and test the automation.
4. Save screenshots of your automation to include in your project portfolio.

---

## 📤 Sharing Your Project
When you’ve completed the automation:
1. Export screenshots of your As-Is & To-Be diagrams from Draw.io.
2. Take screenshots of your Power Automate flow.
3. Push all files to your GitHub repository as part of your bootcamp project.

---

✅ **You’ve now gone from Problem Analysis → Process Design → Automation Development!**  
In the final wrap-up session, we’ll reflect on what you’ve built and how you can apply these skills to real-world jobs.
