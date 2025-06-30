# 📧 IMPROVED EMAIL TEMPLATE FOR EMAILJS

## Copy this HTML template to your EmailJS dashboard:

**Go to:** EmailJS Dashboard → Email Templates → Edit your template → Switch to HTML mode

**Subject:** `New Contact from {{name}} - Enkisoma Website`

**HTML Content:**

```html
<div
  style="font-family: system-ui, sans-serif, Arial; font-size: 14px; background-color: #f8f9fa; padding: 20px;"
>
  <div
    style="max-width: 600px; margin: 0 auto; background: white; border-radius: 10px; overflow: hidden; box-shadow: 0 4px 20px rgba(0,0,0,0.1);"
  >
    <!-- Header -->
    <div
      style="background: linear-gradient(135deg, #4550e6 0%, #7c3aed 100%); padding: 25px; text-align: center;"
    >
      <h1 style="color: white; margin: 0; font-size: 24px; font-weight: 600;">
        📧 New Enkisoma Inquiry
      </h1>
      <p
        style="color: rgba(255,255,255,0.9); margin: 5px 0 0 0; font-size: 16px;"
      >
        Someone is interested in your services!
      </p>
    </div>

    <!-- Content -->
    <div style="padding: 30px;">
      <div
        style="background-color: #f8f9ff; border-left: 4px solid #4550e6; padding: 20px; margin-bottom: 25px; border-radius: 5px;"
      >
        <p
          style="margin: 0; color: #2c3e50; font-size: 16px; font-weight: 500;"
        >
          📝 A message from <strong>{{name}}</strong> has been received. Please
          respond at your earliest convenience.
        </p>
      </div>

      <!-- Contact Details -->
      <div
        style="margin: 25px 0; padding: 20px; border: 1px solid #e1e1e1; border-radius: 8px;"
      >
        <table
          role="presentation"
          style="width: 100%; border-collapse: collapse;"
        >
          <tr>
            <td style="vertical-align: top; width: 60px; padding-right: 15px;">
              <div
                style="width: 50px; height: 50px; background: linear-gradient(135deg, #4550e6, #7c3aed); border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 24px; color: white;"
              >
                👤
              </div>
            </td>
            <td style="vertical-align: top;">
              <div
                style="color: #2c3e50; font-size: 18px; font-weight: 600; margin-bottom: 8px;"
              >
                {{name}}
              </div>
              <div style="color: #666; font-size: 14px; margin-bottom: 4px;">
                📧 <strong>Email:</strong>
                <a
                  href="mailto:{{email}}"
                  style="color: #4550e6; text-decoration: none;"
                  >{{email}}</a
                >
              </div>
              <div style="color: #666; font-size: 14px; margin-bottom: 15px;">
                🏫 <strong>School:</strong> {{school}}
              </div>

              <!-- Message -->
              <div
                style="background: #f8f9fa; padding: 15px; border-radius: 6px; border-left: 3px solid #4550e6;"
              >
                <p
                  style="color: #666; font-size: 14px; margin: 0 0 8px 0; font-weight: 600;"
                >
                  💬 Message:
                </p>
                <p
                  style="font-size: 16px; line-height: 1.5; color: #2c3e50; margin: 0;"
                >
                  {{message}}
                </p>
              </div>
            </td>
          </tr>
        </table>
      </div>

      <!-- Action Button -->
      <div style="text-align: center; margin: 30px 0;">
        <a
          href="mailto:{{email}}?subject=Re: Your Enkisoma Inquiry&body=Dear {{name}},%0D%0A%0D%0AThank you for your interest in Enkisoma Africa's digital education solutions.%0D%0A%0D%0ABest regards,%0D%0AEnkisoma Team"
          style="background: linear-gradient(135deg, #4550e6, #7c3aed); color: white; padding: 15px 30px; text-decoration: none; border-radius: 25px; font-weight: 600; display: inline-block; font-size: 16px;"
        >
          📧 Reply to {{name}}
        </a>
      </div>

      <!-- Footer -->
      <div
        style="border-top: 1px solid #e1e1e1; padding-top: 20px; text-align: center; color: #666; font-size: 14px;"
      >
        <p style="margin: 0 0 10px 0;">
          <strong>Enkisoma Africa</strong> - Transforming African Education
          Through Technology
        </p>
        <p style="margin: 0; font-size: 12px;">
          📍 Senteu Plaza, 6th floor, Galana road, Nairobi | 📞 +254-713-587-950
          | 🌐 www.enkisoma.org
        </p>
      </div>
    </div>
  </div>
</div>
```

## 🎯 How to Update Your EmailJS Template:

1. Go to [EmailJS Dashboard](https://dashboard.emailjs.com/admin) → Email Templates
2. Find your template: `template_04e536h`
3. Click **Edit**
4. Switch to **HTML** mode (toggle in top right)
5. Replace the content with the HTML above
6. Click **Save**
7. Test with your contact form!

## ✅ Features of This Template:

- 📱 Mobile-responsive design
- 🎨 Enkisoma brand colors and styling
- 📧 One-click reply button with pre-filled content
- 🏫 Clear contact information layout
- 💼 Professional business appearance
- 🔗 Direct links to reply and contact info

This will make your contact form emails look extremely professional and branded!
