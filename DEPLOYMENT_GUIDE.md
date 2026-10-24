# Complete Step-by-Step Guide: Launching Maharashtra Pest Control Online

This guide walks you through taking the project files from your local computer and publishing them as a live, secure website accessible to customers across Mumbai, Navi Mumbai, and Thane.

---

## 📁 1. Your Project Structure
All your files are located at:
`C:\Users\user\.gemini\antigravity-ide\scratch\maharashtra-pest-control\`

```
maharashtra-pest-control/
├── index.html          # Main website structure & modals
├── css/
│   └── style.css       # Complete design, responsive layout & styling
├── js/
│   ├── data.js         # Pest data, seed bookings, & storage engine
│   └── app.js          # Booking slot logic (max 2/day), OTP, & admin panel
├── assets/
│   └── images/         # Logos and photo assets
├── README.md           # Project documentation
└── DEPLOYMENT_GUIDE.md # This guide
```

---

## ⚡ 2. Quick Free Hosting Options (Live in Under 5 Minutes)

Because your website is built with clean HTML, CSS, and JavaScript, **it does not require expensive server setups or build steps**. You can host it 100% free with SSL (`https://`).

### Option A: Netlify Drop (Easiest - 2 Minutes, Zero Coding)
1. Open your browser and go to [app.netlify.com/drop](https://app.netlify.com/drop).
2. Sign up or log in (free with Google or GitHub).
3. Open File Explorer to:
   `C:\Users\user\.gemini\antigravity-ide\scratch\`
4. Drag and drop the whole **`maharashtra-pest-control`** folder onto the Netlify drop zone.
5. In 10 seconds, Netlify will generate a live web link (e.g., `https://maharashtra-pest-control.netlify.app`).
6. You can change the site name for free in **Site Settings > Change site name**.

---

### Option B: Vercel (Fast & Professional)
1. Go to [vercel.com](https://vercel.com) and create a free account.
2. Install Vercel CLI in PowerShell or drag/import from GitHub:
   ```powershell
   cd C:\Users\user\.gemini\antigravity-ide\scratch\maharashtra-pest-control
   npx vercel
   ```
3. Follow the 3 prompts by pressing `Enter`. Your site will be published at `https://your-name.vercel.app`.

---

### Option C: GitHub Pages (Free & Reliable)
1. Create a repository on [github.com](https://github.com) named `maharashtra-pest-control`.
2. Push your files to GitHub:
   ```powershell
   cd C:\Users\user\.gemini\antigravity-ide\scratch\maharashtra-pest-control
   git init
   git add .
   git commit -m "Initial Maharashtra Pest Control release"
   git branch -M main
   git remote add origin https://github.com/<YOUR-USERNAME>/maharashtra-pest-control.git
   git push -u origin main
   ```
3. In GitHub repo, go to **Settings > Pages > Source: main branch > Save**.
4. Your website will be live at `https://<YOUR-USERNAME>.github.io/maharashtra-pest-control/`.

---

## 🌐 3. Connecting a Custom Domain (e.g. `maharashtrapestcontrol.com` or `.in`)

To look 100% professional to customers in Mumbai:
1. **Buy a domain name**:
   - Go to [Hostinger](https://hostinger.in), [GoDaddy](https://godaddy.com), or [Namecheap](https://namecheap.com).
   - Search for `maharashtrapestcontrol.in` or `maharashtrapestcontrol.com` (~₹399 to ₹899 per year).
2. **Connect to Netlify or Vercel**:
   - Go to your Netlify/Vercel dashboard > **Domain Management** > **Add Custom Domain**.
   - Enter your domain name (e.g., `maharashtrapestcontrol.com`).
   - Add the two DNS records in your domain registrar's DNS settings:
     - **A Record**: Points to the IP provided by Netlify/Vercel (e.g. `75.2.60.5`).
     - **CNAME Record**: `www` points to your Netlify/Vercel site address.
3. Free SSL (https green lock) is issued automatically within 15 minutes!

---

## 📱 4. Production Integrations (WhatsApp, Phone & Real SMS)

### WhatsApp & Direct Phone Calls
- **Already 100% Live**: Clicking the WhatsApp button or Call button on your site opens directly on customer smartphones to chat with or call **+91 7208102567 (Harshal Satkar)**. No setup required!

### Upgrading to Real SMS OTP (Optional)
The website currently has a built-in real-time SMS simulator toast for instant demo testing. To send real SMS to phones:
1. Create a free account on an Indian SMS Gateway like **[Fast2SMS](https://www.fast2sms.com)** or **[MSG91](https://msg91.com)**.
2. Get your free API Key.
3. Send the OTP code generated in `js/app.js` using their simple 1-line fetch request:
   ```javascript
   fetch(`https://www.fast2sms.com/dev/bulkV2?authorization=YOUR_API_KEY&variables_values=${otp}&route=otp&numbers=${phone}`);
   ```

---

## 💳 5. Receiving Real Payments on +91 7208102567

1. In `index.html` and `js/data.js`, the UPI ID is set to `7208102567@upi`.
2. When customers click to pay on mobile or scan the QR code with Google Pay, PhonePe, or Paytm, the money is credited directly to Harshal Satkar’s bank account linked to `7208102567`.
3. To replace the default SVG QR code with your official bank QR photo:
   - Save your Google Pay/PhonePe QR image as `assets/images/harshal_upi_qr.png`.
   - Update the QR container image in `index.html`.

---

## ☁️ 6. Cloud Database Sync (For Multi-Device Data Sync)

Currently, customer bookings and feedback are saved in the browser’s `localStorage`. To make bookings made on a customer's phone immediately show up on Harshal Satkar's laptop or phone in real time:
- Connect **Firebase Firestore** or **Supabase** (both have generous 100% free tiers):
  1. Go to [firebase.google.com](https://firebase.google.com) and click **Create Project**.
  2. Add **Firestore Database (Test Mode)**.
  3. Include the Firebase CDN script in `index.html`.
  4. Replace `localStorage.setItem` in `js/data.js` with `db.collection('bookings').add(...)`.

---

## 🎯 Summary Checklist
| Step | Action | Time Needed | Cost |
|---|---|---|---|
| **1. Local Testing** | Run `python -m http.server 8080` | Done | Free |
| **2. Free Web Hosting** | Drag folder onto [Netlify Drop](https://app.netlify.com/drop) | 2 mins | Free |
| **3. Custom Domain** | Connect `maharashtrapestcontrol.in` | 10 mins | ~₹499/year |
| **4. Direct WhatsApp** | Active for `7208102567` | Already done | Free |
| **5. UPI QR Code** | Linked to `7208102567@upi` | Already done | Free |
