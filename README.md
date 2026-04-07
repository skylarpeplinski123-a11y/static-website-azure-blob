
🚀 Static Website on Azure Blob Storage

Hosting your first serverless website using Azure ☁️

🎥 Walkthrough Video
https://www.loom.com/share/3414d32d8585444197ffe09edde77fef

🎯 Objective

Deploy your first public-facing website in Azure using Blob Storage instead of a traditional server.

What this teaches:
☁️ PaaS (Platform as a Service)

⚡ Serverless hosting

🧱 Infrastructure handled by Azure

🎨 You focus only on content


🧠 Architecture OverviewUser:

(Internet) ↓ Public URL ↓ Storage Account ↓ $web container  ↓ index.html
      
 
 

⚙️ Prerequisites

-- Azure Subscription (Free Tier OK)

-- Text Editor (Notepad / VS Code / TextEdit)

🧾 Naming Convention
Resource Group: rg-lab01-[yourname]
Storage Account: stlab01[yourname]
Region: East US

⚠️ Rules:

lowercase only
no special characters
must be globally unique

🛠️ Deployment Steps

🔹 Phase 1: Create Resource Group

Go to: https://portal.azure.com
Search: Resource Groups
Click + Create

Fill in:

Resource Group → rg-lab01-[yourname]
Region → East US

👉 Click Review + Create → Create


🔹 Phase 2: Create Storage Account

Search: Storage Accounts
Click + Create

Fill in:
--Resource Group → rg-lab01-[yourname]
--Name → stlab01[yourname]
--Region → East US
--Performance → Standard
--Redundancy → LRS

👉 Click Review + Create → Create

⏱️ Wait → Click Go to resource


🔹 Phase 3: Enable Static Website

--Go to Static website (left menu)
--Set → Enabled
--Index document: index.html
--Error document: 404.html

👉 Click Save

📌 Copy your Primary Endpoint URL
(this is your live website)


🔹 Phase 4: Create Website File

Create a file called: index.html


Paste this:

<!DOCTYPE html>
<html>
<head>
<title>My First Cloud Site</title>
<style>
body {
  font-family: sans-serif;
  text-align: center;
  margin-top: 50px;
  background-color: #f0f0f0;
}
h1 { color: #0078d4; }
</style>
</head>
<body>
<h1>Hello from the Cloud!</h1>
<p>This site is hosted on Azure Blob Storage.</p>
<p>Deployed by: [Your Name]</p>
</body>
</html>

