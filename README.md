# static-website-azure-blob
Hosting first Static Website with Azure
🚀 Azure Blob Static Website (Super Simple Guide)

🎥 Watch this first (quick walkthrough):
👉 https://www.loom.com/share/3414d32d8585444197ffe09edde77fef

🧠 What is this?

This is a super simple static website hosted using:

Microsoft Azure Blob Storage
HTML, CSS, JavaScript
No servers needed

Think of it like:

putting website files into a magic online folder ☁️

📁 What’s inside this repo?
index.html   → the main page
styles.css   → makes it look nice
script.js    → adds small interactions
404.html     → error page
🧒 Step-by-step (explained like you're 5)
🟢 Step 1 — Download these files

Click the green Code button → Download ZIP
OR clone the repo

🟢 Step 2 — Go to Azure

Open Microsoft Azure

🟢 Step 3 — Create a Storage Account

Search: Storage Accounts
Click Create

🟢 Step 4 — Turn on Static Website

Inside your storage account:

Click Static website
Turn it ON

Fill in:

Index document name: index.html
Error document path: 404.html

Click Save

🟢 Step 5 — Find the magic folder

Azure creates a special container called:

$web
🟢 Step 6 — Upload your files

Upload ALL of these into $web:

index.html
styles.css
script.js
404.html
🟢 Step 7 — Open your website 🎉

Azure gives you a link like:

https://yourstorage.z13.web.core.windows.net/

Click it → your site is LIVE

⚠️ VERY IMPORTANT

File names must match EXACTLY:

index.html  ✅
Index.html  ❌
INDEX.HTML ❌

Azure is case-sensitive.
