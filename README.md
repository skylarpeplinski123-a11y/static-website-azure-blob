# static-website-azure-blob
Hosting first Static Website with Azure

🚀 Azure Static Website Lab (Blob Storage)

🎥 Quick Walkthrough
https://www.loom.com/share/3414d32d8585444197ffe09edde77fef

🎯 Objective

Deploy your first public website in Azure using:

☁️ Azure Blob Storage
⚡ Serverless hosting
🧱 PaaS (no servers needed)

You focus on the website — Azure handles everything else

🧠 Architecture
Internet User
     ↓
Public URL
     ↓
Storage Account
     ↓
$web container
     ↓
index.html
⚙️ Requirements
Azure account (Free Tier OK)
Text editor (Notepad / VS Code)
🧾 Naming Standard
Resource Group: rg-lab01-[yourname]
Storage Account: stlab01[yourname]
Region: East US

⚠️ Must be:

lowercase
globally unique
🛠️ Deployment Steps
1️⃣ Create Resource Group
Go to: https://portal.azure.com
Resource Groups → Create
Name: rg-lab01-[yourname]
2️⃣ Create Storage Account
Storage Accounts → Create
Name: stlab01[yourname]
Performance: Standard
Redundancy: LRS
3️⃣ Enable Static Website
Open Static website
Enable it
Index: index.html
Error: 404.html

📌 Copy your Primary Endpoint URL

4️⃣ Create Your Site

Save as index.html:

<h1>🚀 Hello from the Cloud!</h1>
<p>This site is hosted on Azure Blob Storage.</p>
5️⃣ Upload Files
Go to Containers
Open $web
Upload index.html
6️⃣ Validate
Open your URL
Your site should be live 🎉
⚠️ Troubleshooting

404 error

Must be index.html (exact name)
Must be inside $web

Storage name taken

Add numbers → stlab01john99
🧹 Clean Up
Resource Groups
Select your group
Delete

Blob Storage
Static hosting
No infrastructure
