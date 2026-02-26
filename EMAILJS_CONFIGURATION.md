# EmailJS Configuration - Bharat Solar Contact Form

## ✅ UPDATED CREDENTIALS (Correct)

### EmailJS Account Details:
- **Email:** bharatpowersolarenergy4@gmail.com
- **Public Key:** Q1ORcKRr0ZcPE8pCK
- **Private Key:** MzGsbuHpYpfCYxgZEYFMX (Keep secret!)
- **Service ID:** service_7e3n37v
- **Template ID:** template_x82fage

---

## 📋 Form Fields

The contact form collects the following information:

1. **name** - Customer's full name
2. **email** - Customer's email address
3. **phone** - Customer's phone number
4. **capacity** - Solar system capacity (e.g., 3 HP, 5 HP, 10 HP)
5. **message** - Customer's inquiry/requirements

---

## 🔧 Integration Status

✅ EmailJS library loaded from CDN
✅ Public key configured correctly
✅ Service ID updated to: service_7e3n37v
✅ Template ID updated to: template_x82fage
✅ Form submission handler implemented
✅ Success/error messages configured
✅ Form reset after successful submission
✅ Loading state during submission

---

## 📧 Email Template Variables

Make sure your EmailJS template (template_x82fage) includes these variables:

```
{{name}}      - Customer name
{{email}}     - Customer email
{{phone}}     - Customer phone number
{{capacity}}  - Solar system capacity
{{message}}   - Customer message
```

### Recommended Template Format:

**Subject:** New Solar Inquiry from {{name}}

**Body:**
```
Hello Bharat Solar Team,

You have received a new inquiry from your website contact form:

Customer Details:
- Name: {{name}}
- Email: {{email}}
- Phone: {{phone}}
- Solar System Capacity: {{capacity}}

Customer Message:
{{message}}

---
Please respond to this inquiry as soon as possible.

This email was automatically sent from the Bharat Solar website contact form.
```

---

## 🧪 Testing the Form

1. Open your website: http://127.0.0.1:5500/contact.html
2. Fill out all form fields with test data
3. Click "Get Free Quote" button
4. Watch for success message: "✓ Thank you! Your inquiry has been sent successfully..."
5. Check your email: bharatpowersolarenergy4@gmail.com
6. Verify the email arrived with all form data

---

## 🐛 Troubleshooting

### If form submission fails:

1. **Check Browser Console (F12)**
   - Look for error messages
   - Verify EmailJS is loaded
   - Check for JavaScript errors

2. **Verify EmailJS Dashboard**
   - Login to https://dashboard.emailjs.com/
   - Check that service is connected
   - Verify template exists
   - Ensure account is verified

3. **Common Issues:**
   - Service not connected to Gmail
   - Template variables don't match form fields
   - Account not verified
   - Incorrect credentials

---

## 📱 Contact Information

If customers can't submit the form, they can contact directly:

- **Email:** bharatpowersolarenergy4@gmail.com
- **Phone:** +91 8308067878
- **Address:** Shree venktesh society, near chetak ghoda, ch.sambhanjinagar

---

## 🔒 Security Notes

- ✅ Public key is safe to use in client-side code
- ⚠️ Private key should NEVER be exposed in client-side code
- ✅ EmailJS handles email sending securely
- ✅ Form includes spam protection via EmailJS

---

## 📊 Email Delivery

Emails will be sent to: **bharatpowersolarenergy4@gmail.com**

- Check inbox for new inquiries
- Check spam folder if emails don't arrive
- Set up email filters to organize inquiries
- Consider setting up auto-reply for customers

---

**Configuration Date:** February 25, 2026
**Status:** ✅ Active and Ready
