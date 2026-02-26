# EmailJS Template Code - Bharat Solar Contact Form

## 📧 Template ID: template_x82fage

---

## 🎯 COPY THIS CODE TO EMAILJS TEMPLATE

### Step 1: Go to EmailJS Dashboard
1. Login to https://dashboard.emailjs.com/
2. Click on "Email Templates" in the left menu
3. Find your template: **template_x82fage**
4. Click "Edit" button

---

### Step 2: Email Settings

**To Email:** bharatpowersolarenergy4@gmail.com

**From Name:** Bharat Solar Website

**From Email:** {{email}}

**Reply To:** {{email}}

**Subject:** New Solar Inquiry from {{name}} - {{capacity}}

---

### Step 3: Content (HTML Template)

**Copy and paste this EXACT code into the "Content" section:**

```html
<div style="font-family: system-ui, sans-serif, Arial; font-size: 12px">
    <div>A message by {{name}} has been received. Kindly respond at your earliest convenience.</div>
    
    <div style="margin-top: 20px; padding: 15px 0; border-width: 1px 0; border-style: dashed; border-color: lightgrey;">
        <table role="presentation">
            <tr>
                <td style="vertical-align: top">
                    <div style="padding: 6px 10px; margin: 0 10px; background-color: aliceblue; border-radius: 5px; font-size: 26px;" role="img">👤</div>
                </td>
                <td style="vertical-align: top">
                    <div style="color: #2c3e50; font-size: 16px"><strong>{{name}}</strong></div>
                    <div style="color: #999999; font-size: 13px; margin-top: 5px;">📅 {{time}}</div>
                    <div style="color: #555; font-size: 13px; margin-top: 5px;">📞 {{mobile}}</div>
                    <div style="color: #555; font-size: 13px; margin-top: 5px;">📧 {{email}}</div>
                    <div style="color: #555; font-size: 13px; margin-top: 5px;">⚡ Solar Capacity: {{capacity}}</div>
                    <p style="font-size: 16px; margin-top: 15px; color: #333;">{{message}}</p>
                </td>
            </tr>
        </table>
    </div>
    
    <div style="margin-top: 20px; padding: 15px; background-color: #f8f9fa; border-left: 4px solid #2ecc71; border-radius: 5px;">
        <p style="margin: 0; font-size: 14px; color: #555;">
            <strong style="color: #2ecc71;">📋 Quick Summary:</strong><br>
            <strong>Name:</strong> {{name}}<br>
            <strong>Email:</strong> {{email}}<br>
            <strong>Phone:</strong> {{mobile}}<br>
            <strong>Solar System:</strong> {{capacity}}<br>
            <strong>Received:</strong> {{time}}
        </p>
    </div>
    
    <div style="margin-top: 20px; padding: 10px; background-color: #fff3cd; border-radius: 5px; font-size: 13px; color: #856404;">
        ⚠️ <strong>Action Required:</strong> Please respond to this inquiry within 24 hours for best customer service.
    </div>
    
    <div style="margin-top: 30px; padding-top: 20px; border-top: 1px solid #e0e0e0; font-size: 11px; color: #999;">
        <p style="margin: 0;">This email was automatically sent from the Bharat Solar website contact form.</p>
        <p style="margin: 5px 0 0 0;">🌐 Website: www.bharatsolar.com | 📞 +91 8308067878</p>
    </div>
</div>
```

---

### Step 4: Template Variables Used

Make sure these variables are available in your template:

| Variable | Description | Source |
|----------|-------------|--------|
| `{{name}}` | Customer's full name | Form field: name |
| `{{email}}` | Customer's email address | Form field: email |
| `{{mobile}}` | Customer's phone number | Form field: phone |
| `{{capacity}}` | Solar system capacity | Form field: capacity |
| `{{message}}` | Customer's inquiry message | Form field: message |
| `{{time}}` | Submission date and time | Auto-generated (Indian time) |

---

### Step 5: Test Template

After saving the template:

1. Click "Test it" button in EmailJS dashboard
2. Fill in sample values for all variables
3. Send test email
4. Check bharatpowersolarenergy4@gmail.com inbox
5. Verify all fields display correctly

---

## 📱 Sample Test Data

Use this data to test your template:

```
name: Ajay Dhore
email: ajaydhore96@gmail.com
mobile: 9623898178
capacity: 5 HP Solar System
message: I am interested in installing a 5 HP solar system for my home. Please provide a quote and installation timeline.
time: Feb 25, 2026, 02:30 PM
```

---

## ✅ Verification Checklist

- [ ] Template ID is: template_x82fage
- [ ] Service ID is: service_7e3n37v
- [ ] Public Key is: Q1ORcKRr0ZcPE8pCK
- [ ] "To Email" is set to: bharatpowersolarenergy4@gmail.com
- [ ] All 6 variables are included: name, email, mobile, capacity, message, time
- [ ] HTML template is pasted correctly
- [ ] Test email sent successfully
- [ ] Email received in inbox (check spam if not)
- [ ] All fields display properly in received email

---

## 🎨 Email Preview

When you receive an email, it will look like:

```
Subject: New Solar Inquiry from Ajay Dhore - 5 HP Solar System

Body:
┌─────────────────────────────────────────────┐
│ A message by Ajay Dhore has been received. │
│ Kindly respond at your earliest convenience.│
├─────────────────────────────────────────────┤
│ 👤  Ajay Dhore                              │
│     📅 Feb 25, 2026, 02:30 PM               │
│     📞 9623898178                            │
│     📧 ajaydhore96@gmail.com                │
│     ⚡ Solar Capacity: 5 HP Solar System    │
│                                              │
│     I am interested in installing a 5 HP    │
│     solar system for my home...             │
├─────────────────────────────────────────────┤
│ 📋 Quick Summary:                           │
│ Name: Ajay Dhore                            │
│ Email: ajaydhore96@gmail.com                │
│ Phone: 9623898178                           │
│ Solar System: 5 HP Solar System             │
│ Received: Feb 25, 2026, 02:30 PM            │
└─────────────────────────────────────────────┘
```

---

## 🔧 Troubleshooting

**If variables don't show:**
- Make sure variable names match exactly (case-sensitive)
- Check for typos in {{variable}} syntax
- Verify form field names match template variables

**If email doesn't arrive:**
- Check spam/junk folder
- Verify "To Email" is correct
- Check EmailJS dashboard for delivery status
- Ensure Gmail service is connected

---

**Last Updated:** February 25, 2026
**Status:** ✅ Ready to Use
