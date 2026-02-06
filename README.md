# 🛠 Setup Guide

Follow these steps to get started:

1. **Set up the Lead Machine Form**
   Customize the form fields (Business Type, Location, Lead Number, Email Style) in the **Form Trigger** node. This is how you collect the target lead criteria.

2. **Plug in your [Apify](https://apify.com/) API endpoint**
   Replace `Apify_Actor_Endpoint_URL` in the **HTTP Request** node with your own Apify actor URL to scrape business data.

3. **Add your [Google Gemini](https://aistudio.google.com/apikey) credentials**
   This is used in the **Information Extractor** node to find the best email address from a business website.

4. **Connect your [Google Sheets](https://docs.google.com/spreadsheets/)**
   Link the sheet in both **Append row** and **Append/Update row** nodes. Make sure your sheet has columns for Company Name, Website, Phone, Email, Address, Category, Cold Mail Status, and Send Time.

5. **Add your [OpenAI](https://platform.openai.com/) API key**
   This powers the cold email generation in the **Information Extractor1** node for subject & body creation.

6. **Connect your [Gmail](https://mail.google.com/) account**
   In the **Send a message** node, link your Gmail account to send the cold emails automatically.

Once all connections are set, your workflow will **collect leads, store them, and send cold emails automatically** 🚀
