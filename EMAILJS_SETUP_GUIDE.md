# EmailJS Setup Guide for Bharat Solar Contact Form

## What is EmailJS?
EmailJS allows you to send emails directly from your website's contact form without needing a backend server. All form submissions will be sent directly to your email address.

## Setup Steps

### Step 1: Create EmailJS Account
1. Go to [https://www.emailjs.com/](https://www.emailjs.com/)
2. Click "Sign Up" and create a free account
3. Verify your email address

### Step 2: Add Email Service
1. After logging in, go to "Email Services" in the dashboard
2. Click "Add New Service"
3. Choose your email provider (Gmail recommended)
4. For Gmail:
   - Click "Connect Account"
   - Sign in with your Gmail account: **bharatpowersolarenergy4@gmail.com**
   - Allow EmailJS to access your account
5. Give your service a name (e.g., "Bharat Solar Gmail")
6. Click "Create Service"
7. **IMPORTANT**: Copy the "Service ID" (you'll need this later)

### Step 3: Create Email Template
1. Go to "Email Templates" in the dashboard
2. Click "Create New Template"
3. Use this template content:

**Template Name**: Solar Quote Request

**Subject**: New Solar Quote Request from {{name}}

**Content**:
```
New Solar Quote Request

Customer Details:
- Name: {{name}}
- Email: {{email}}
- Phone: {{phone}}
- Solar System Capacity: {{capacity}}

Message:
{{message}}

---
This inquiry was submitted from the Bharat Solar website contact form.
```

4. Click "Save"
5. **IMPORTANT**: Copy the "Template ID" (you'll need this later)

### Step 4: Get Your Public Key
1. Go to "Account" in the dashboard
2. Find "API Keys" section
3. **IMPORTANT**: Copy your "Public Key"

### Step 5: Update Your Website
Open the file `solar/contact.html` and replace these three values:

1. Find `YOUR_PUBLIC_KEY` and replace with your actual Public Key
2. Find `YOUR_SERVICE_ID` and replace with your Service ID
3. Find `YOUR_TEMPLATE_ID` and replace with your Template ID

**Example:**
```javascript
emailjs.init("abc123xyz"); // Your Public Key
emailjs.sendForm('service_abc123', 'template_xyz789', this)
```

### Step 6: Test Your Form
1. Open your website in a browser
2. Go to the Contact page
3. Fill out the form with test data
4. Click "Get Free Quote"
5. Check your email (bharatpowersolarenergy4@gmail.com) for the test submission

## Free Plan Limits
- 200 emails per month
- Perfect for a small to medium business
- If you need more, you can upgrade to a paid plan

## Troubleshooting

### Not receiving emails?
1. Check your spam/junk folder
2. Verify all three IDs are correctly entered in contact.html
3. Check the browser console for error messages (F12 key)
4. Make sure your EmailJS service is connected and active

### Form not submitting?
1. Open browser console (F12) and check for errors
2. Verify the EmailJS script is loading (check Network tab)
3. Make sure you initialized EmailJS with your Public Key

## Alternative: Google Forms
If you prefer a simpler solution without coding:
1. Create a Google Form
2. Get the form embed code
3. Replace the contact form section with the Google Form iframe

## Support
- EmailJS Documentation: https://www.emailjs.com/docs/
- EmailJS Support: support@emailjs.com

---
**Note**: Keep your Service ID, Template ID, and Public Key secure. Don't share them publicly.
