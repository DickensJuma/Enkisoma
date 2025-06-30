# 📧 Contact Form Setup Instructions

Your contact form is ready and just needs EmailJS configuration to work. Follow these steps:

## 🚀 Quick Setup (5 minutes)

### 1. Get EmailJS Account

- Go to [https://www.emailjs.com/](https://www.emailjs.com/)
- Sign up for FREE (no credit card required)
- Verify your email

### 2. Add Email Service

**IMPORTANT: Gmail API Scope Fix**

- Dashboard → Email Services → Add New Service
- Choose your email provider (Gmail recommended)
- **When connecting Gmail, make sure to:**
  1. Click "Advanced" if you see a warning
  2. Allow ALL permissions requested (including "Send email on your behalf")
  3. If you get "insufficient authentication scopes" error:
     - Go back to Email Services
     - Delete the Gmail service
     - Add it again and grant ALL permissions
- Connect your `info@enkisoma.org` email
- Copy the **Service ID** (looks like: `service_abc123`)

**Alternative Email Services (if Gmail issues persist):**

- Outlook/Hotmail (often easier setup)
- Yahoo Mail
- Custom SMTP (advanced users)

### 3. Create Email Template

- Dashboard → Email Templates → Create New Template
- Template Name: `enkisoma_contact`
- Subject: `New Contact from {{name}} - Enkisoma Website`
- Content:

```
New message from Enkisoma website:

Name: {{name}}
Email: {{email}}
School: {{school}}

Message:
{{message}}

Reply to: {{email}}
```

- Save and copy the **Template ID** (looks like: `template_xyz789`)

### 4. Get Public Key

- Dashboard → Account → General
- Copy your **Public Key** (looks like: `user_abcdefghijk123`)

### 5. Update Website Code

Open `index.html` and find these 3 lines around line 3569:

**Line ~3569:** Replace `YOUR_PUBLIC_KEY`

```javascript
emailjs.init("user_YOUR_ACTUAL_PUBLIC_KEY");
```

**Line ~3594:** Replace both IDs

```javascript
emailjs.send("service_YOUR_SERVICE_ID", "template_YOUR_TEMPLATE_ID", formData);
```

## 🎯 Example Configuration

```javascript
// Example of what your final code should look like:
emailjs.init("user_abcd1234567890");
emailjs.send("service_gmail", "template_contact", formData);
```

## ✅ Testing

1. Save the file
2. Open website in browser
3. Fill out contact form
4. Submit - you should receive email at info@enkisoma.org

## 🆘 Troubleshooting

**Gmail API "insufficient authentication scopes" error?**

1. Go to EmailJS Dashboard → Email Services
2. Delete your Gmail service
3. Add Gmail service again
4. When authorizing, click "Advanced" → "Go to EmailJS (unsafe)"
5. Grant ALL permissions including "Send email on your behalf"
6. Test again

**Form not sending?**

- Check browser console (F12) for errors
- Verify all 3 IDs are correct (no quotes missing)
- Make sure EmailJS service is connected

**Not receiving emails?**

- Check spam folder
- Verify template variables match: `{{name}}`, `{{email}}`, `{{school}}`, `{{message}}`
- Test EmailJS template directly in dashboard

**EmailJS fails completely?**

- The form has a built-in fallback that opens the user's email client
- They can still send emails manually to info@enkisoma.org

## 📱 Current Features

✅ Responsive design
✅ Form validation  
✅ Loading states
✅ Success/error messages
✅ EmailJS integration
✅ Mailto fallback
✅ Accessibility compliant

Your contact form is professional-grade and ready to handle inquiries from schools interested in Enkisoma's services!
