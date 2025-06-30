# 🔧 Gmail API Scope Error - Fix Guide

## Problem

EmailJS error: "Request had insufficient authentication scopes" when using Gmail

## ⚡ Quick Fix (2 minutes)

### Step 1: Re-authenticate Gmail

1. Go to [EmailJS Dashboard](https://dashboard.emailjs.com/admin)
2. Click **Email Services** in sidebar
3. Find your Gmail service → Click **Delete** ❌
4. Click **Add New Service** → Choose **Gmail**

### Step 2: Grant Full Permissions

When Gmail authorization popup appears:

1. ✅ **Don't click "Advanced"** - just proceed normally
2. If you see "This app isn't verified":
   - Click **Advanced**
   - Click **Go to EmailJS (unsafe)**
3. ✅ **Grant ALL permissions** including:
   - Read email
   - **Send email on your behalf** ← This is crucial!
   - Manage drafts

### Step 3: Test Immediately

- Use the `emailjs-test.html` file
- Send a test email
- Check `info@enkisoma.org` inbox

## 🎯 Alternative Solutions

### Option A: Use Outlook Instead

- Often has fewer permission issues
- Works exactly the same way
- Go to Email Services → Add New → Outlook

### Option B: Use App-Specific Password (Advanced)

1. Enable 2FA on Gmail account
2. Generate app-specific password
3. Use SMTP service in EmailJS with app password

### Option C: Business Gmail Account

- Google Workspace accounts have fewer restrictions
- Better for business use anyway

## 🔍 How to Verify It's Working

### Test in Browser Console:

1. Open website → Press F12 → Go to Console
2. Fill out contact form and submit
3. Look for:
   - ✅ "SUCCESS!" message = Working
   - ❌ "FAILED" + error = Still broken

### Test Email Receipt:

- Check `info@enkisoma.org` inbox
- Check spam folder
- Email should arrive within 30 seconds

## 💡 Pro Tips

1. **Use the same Google account** for EmailJS that owns info@enkisoma.org
2. **Clear browser cache** after re-authentication
3. **Test immediately** after setup (don't wait)
4. **Keep the test page handy** for quick debugging

## 🚨 If Still Not Working

Your contact form has a **built-in backup**:

- If EmailJS fails, it opens user's email client
- They can still send emails to info@enkisoma.org
- No inquiries are lost!

## ✅ Expected Result

After fix: Contact form sends emails directly to info@enkisoma.org with professional formatting and immediate delivery.
