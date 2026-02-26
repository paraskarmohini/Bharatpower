# EmailJS Troubleshooting Guide for Bharat Solar

## Current Error: "Account not found" (404)

This error means EmailJS cannot find your account, service, or template. Follow these steps to fix it:

---

## Step 1: Verify Your EmailJS Account

1. Go to https://dashboard.emailjs.com/
2. Log in with your account (bharatpowersolarenergy4@gmail.com)
3. Make sure your account is **verified** (check your email for verification link)

---

## Step 2: Check Your Email Service

1. In EmailJS dashboard, go to **"Email Services"** in the left menu
2. You should see your Gmail service with ID: **service_7e3n37v**
3. Make sure it shows as **"Connected"** with bharatpowersolarenergy4@gmail.com
4. If not connected:
   - Click on the service
   - Click "Connect Account"
   - Authorize with your Gmail account
   - Make sure to check "Send email on your behalf" permission

---

## Step 3: Verify Your Email Template

1. In EmailJS dashboard, go to **"Email Templates"** in the left menu
2. You should see a template called **"Contact Us"** with ID: **template_2l5mt5p**
3. Click on it to edit and make sure it has these variables:
   - `{{name}}` - Customer name
   - `{{email}}` - Customer email
   - `{{phone}}` - Customer phone number
   - `{{capacity}}` - Solar system capacity
   - `{{message}}` - Customer message

### Recommended Template Content:

**Subject:** New Solar Inquiry from {{name}}

**Body:**
```
Hello Bharat Solar Team,

You have received a new inquiry from your website:

Name: {{name}}
Email: {{email}}
Phone: {{phone}}
Solar System Capacity: {{capacity}}

Message:
{{message}}

---
This email was sent from the Bharat Solar contact form.
```

4. Click **"Save"** after editing

---

## Step 4: Check Your Public Key

1. In EmailJS dashboard, go to **"Account"** → **"General"**
2. Find your **Public Key**: Q1ORcKtr0ZcPE8pCK
3. Make sure this matches the key in your website code

---

## Step 5: Test the Integration

After completing the above steps:

1. Go to your website contact page
2. Fill out the form with test data
3. Submit the form
4. Check the browser console (F12) for any error messages
5. Check your email (bharatpowersolarenergy4@gmail.com) for the test message

---

## Common Issues and Solutions

### Issue 1: "Account not found"
**Solution:** Your EmailJS account might not be verified. Check your email for a verification link from EmailJS.

### Issue 2: "Service not found"
**Solution:** 
- Make sure service ID is exactly: `service_7e3n37v`
- Verify the service is connected to your Gmail account
- Try disconnecting and reconnecting the Gmail service

### Issue 3: "Template not found"
**Solution:**
- Make sure template ID is exactly: `template_2l5mt5p`
- Verify the template exists and is saved
- Check that all template variables match the form field names

### Issue 4: Gmail not receiving emails
**Solution:**
- Check your Gmail spam folder
- Verify the "To Email" in your EmailJS service settings
- Make sure Gmail permissions are granted (send on behalf)

---

## Alternative: Create New Service and Template

If the above doesn't work, create fresh credentials:

### Create New Email Service:
1. Go to "Email Services" → "Add New Service"
2. Select "Gmail"
3. Connect your Gmail account (bharatpowersolarenergy4@gmail.com)
4. Note the new Service ID (e.g., service_xxxxx)

### Create New Email Template:
1. Go to "Email Templates" → "Create New Template"
2. Name it "Contact Form"
3. Add the template content (see above)
4. Note the new Template ID (e.g., template_xxxxx)

### Update Website Code:
Replace the IDs in contact.html:
- Line 681: `emailjs.send('YOUR_NEW_SERVICE_ID', 'YOUR_NEW_TEMPLATE_ID', formData)`

---

## Contact EmailJS Support

If issues persist:
- Email: support@emailjs.com
- Documentation: https://www.emailjs.com/docs/

---

## Current Configuration

- **Public Key:** Q1ORcKRr0ZcPE8pCK
- **Private Key:** MzGsbuHpYpfCYxgZEYFMX (Keep this secret!)
- **Service ID:** service_7e3n37v
- **Template ID:** template_x82fage
- **Email:** bharatpowersolarenergy4@gmail.com
- **Website:** Bharat Solar Contact Form

---

**Last Updated:** February 25, 2026
