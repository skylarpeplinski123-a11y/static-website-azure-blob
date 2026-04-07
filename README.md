# static-website-azure-blob
Hosting first Static Website with Azure

Lab 01: Hosting Your First Static Website in Azure 
https://www.loom.com/share/3414d32d8585444197ffe09edde77fef
 
1. Objective 
In this lab, you will deploy your first public-facing resource in Azure. Instead of building a 
complex server to host a simple website, you will use Azure Blob Storage. This introduces you 
to the concept of PaaS (Platform as a Service) and Serverless hosting, where you focus on 
the content, and Azure handles the infrastructure. 



2. Architecture Diagram 
(Imagine a simple diagram: User (Internet) -> Public URL -> Azure Storage Account ($web 
container) -> index.html) 


3. Prerequisites 
● [ ] Active Azure Subscription (Free Tier is fine). 
● [ ] Completed Week 1 Video Modules. 
● [ ] A basic text editor (Notepad, TextEdit, or VS Code). 


4. Lab Variables (Naming Convention) 
Use these names to ensure consistency. 
● Resource Group: rg-lab01-[yourname] 
● Location: East US 
● Storage Account Name: stlab01[yourname] 
○ Note: Storage account names must be globally unique, all lowercase, and no 
special characters. 


5. Step-by-Step Instructions 


Phase 1: Create the Resource Group 
1. Log in to the Azure Portal (https://www.google.com/search?q=portal.azure.com). 
2. Search for Resource Groups in the top search bar. 
3. Click + Create. 
4. Basics Tab: 
○ Subscription: Select your subscription. 
○ Resource Group: Enter rg-lab01-[yourname]. 
○ Region: Select (US) East US. 
5. Click Review + create -> Create. 


Phase 2: Create the Storage Account 
1. Search for Storage accounts in the search bar. 
2. Click + Create. 
3. Basics Tab: 
○ Resource Group: Select rg-lab01-[yourname]. 
○ Storage account name: stlab01[yourname] (e.g., stlab01jhante). 
Remember: All lowercase, numbers and letters only. 
○ Region: (US) East US. 
○ Performance: Standard. 
○ Redundancy: Locally-redundant storage (LRS). This is the cheapest option for 
labs. 
4. Click Review + create. 
5. Wait for validation to pass, then click Create. 
6. When deployment finishes (about 30 seconds), click Go to resource. 


Phase 3: Enable Static Website Hosting 
1. On the left-hand menu of your Storage Account, look under the Data management 
section. 
2. Click on Static website. 
3. Static website: Switch from "Disabled" to Enabled. 
4. Index document name: Enter index.html. 
5. Error document path: Enter 404.html (Optional, but good practice). 
6. Click Save. 
7. CRITICAL: Once saved, a Primary endpoint URL will appear (e.g., 
https://stlab01jhante.z13.web.core.windows.net/). Copy this URL. This 
is your website's address. 


Phase 4: Create Your Website File 
1. Open your text editor on your computer. 
Paste the following simple HTML code: 
<!DOCTYPE html> 
<html> 
<head> 
<title>My First Cloud Site</title> 
<style> 
body { font-family: sans-serif; text-align: center; margin-top: 50px; background-color: 
#f0f0f0; } 
h1 { color: #0078d4; } 
</style> 
</head> 
<body> 
<h1>Hello from the Cloud!</h1> 
<p>This site is hosted on Azure Blob Storage.</p> 
<p>Deployed by: [Your Name]</p> 
</body> 
</html> 
2.  
3. Save this file on your desktop as index.html. 


Phase 5: Upload Content 
1. Go back to the Azure Portal (you should still be on the Static website blade). 
2. On the left menu, click on Containers (under Data storage). 
3. You will see a new container named $web. This was created automatically. Click to open 
it. 
4. Click Upload at the top. 
5. Browse for your index.html file on your desktop. 
6. Click Upload. 


Phase 6: Validation 
1. Open a new browser tab. 
2. Paste the Primary endpoint URL you copied in Phase 3. 
3. Hit Enter. 
4. You should see your "Hello from the Cloud!" message. 
5. Congratulations! You just deployed a serverless website. 

6. Troubleshooting / Common Issues 

● Issue: "404 - The requested content does not exist." 
○ Fix: Did you name the file exactly index.html? Azure is case-sensitive. 
Index.html or index.txt will not work. 

○ Fix: Did you upload the file to the $web container? If you uploaded it to a 
different container, it won't work. 
● Issue: "Storage account name is already taken." 

○ Fix: Storage names must be unique across all of Azure, not just your account. 
Add some random numbers to the end of your name (e.g., stlab01jhante99). 


7. Clean Up Resources 
Important: Always clean up to keep your cloud environment tidy. 
1. Go to Resource Groups. 
2. Click rg-lab01-[yourname]. 
3. Click Delete resource group. 
4. Type the name to confirm. 
5. Click Delete.
