# MAHARASHTRA PEST CONTROL - Official Web Application

**Proprietor:** Harshal Satkar  
**Contact:** +91 7208102567  
**Email:** maharashtra.pestcontrol13@gmail.com  
**Service Coverage:** Mumbai, Navi Mumbai, Thane and nearby areas (MMR)  
**Experience:** 10+ Years of Certified Pest Control (Established 2014)  

---

## 🌟 Key Application Features

### 1. Dual Interface Architecture
- **Customer / User Interface:**
  - Modern, responsive landing page with treatment details for **Cockroaches, Termites, Bedbugs, Ants, and Rodents**.
  - **Inspection Slot Booking Engine:**
    - Choice of **Household (Residential)** vs **Non-Household (Commercial / Industrial)** premises.
    - Customer inputs Name, Mobile Number, City, and Detailed Address.
    - **Max 2 Slots Per Day Quality Standard:** Strict slot capacity logic (Slot 1: Morning 10 AM - 1 PM, Slot 2: Afternoon/Evening 3 PM - 6 PM). If both slots are booked on any date, system warns the user and prevents overbooking.
    - **Real-Time Mobile OTP:** Simulated interactive instant SMS banner with 1-click autofill for instant number verification.
  - **1-Year Validity AMC Warranty Pass & Track Record:**
    - Displays official digital warranty certificate with start date, 365-day expiry date, and live remaining days countdown.
    - Timeline track record of all technician visits (Initial inspection, drill-fill barrier, quarterly audits).
    - 1-Click WhatsApp Free Recall button & Print Certificate option.
  - **Pre-Payment Portal:**
    - Live branded UPI QR Code for **Harshal Satkar (7208102567@upi)** with PhonePe, Google Pay, Paytm, and BHIM support.
    - Instant digital receipt and automatic payment ledger sync.
  - **Direct Contact Hotlines:**
    - Sticky floating WhatsApp button with pre-filled message.
    - Direct phone call link (`tel:7208102567`).
  - **Customer Feedback & Reviews:**
    - Interactive star rating and review submission.
    - Live feed of verified customer reviews across Mumbai, Navi Mumbai, and Thane.

- **Admin Portal (Harshal Satkar's Control Room):**
  - **Secure Admin OTP Login:** Authenticates using Harshal Satkar's registered phone `7208102567` with simulated SMS alert.
  - **Live Dashboard Metrics:** Total bookings, today's capacity (x/2 slots), active 1-year AMCs, and pre-payments total.
  - **1-Year Validity Expiry Alert Hub:**
    - Automatically highlights customers whose 1-year AMC expires within 30 days or has expired.
    - 1-Click **"Send WhatsApp Renewal Reminder"** with personalized pre-filled discount message.
    - 1-Click **"Renew 1-Year AMC"** button extending validity by another 365 days.
  - **Slot Booking Ledger:** Manage all appointments, mark status (Confirmed, Inspected, Completed), call or WhatsApp customers directly.
  - **Pre-Payments Ledger:** Complete log of all UPI pre-payments received on Harshal Satkar's phone `7208102567`.
  - **Customer Feedback Manager:** View and moderate customer testimonials.

---

## 🚀 How to Run Locally

1. Open PowerShell / Terminal in project directory:
   ```powershell
   cd C:\Users\user\.gemini\antigravity-ide\scratch\maharashtra-pest-control
   ```
2. Start the local HTTP server:
   ```powershell
   python -m http.server 8080
   ```
3. Open your browser and navigate to:
   ```
   http://localhost:8080
   ```

---

## 🔑 Demo Credentials & Quick Test Data

- **Admin Login:** click "Admin Portal" and sign in with your admin username/password (see ADMIN_SECURITY.md).

- **Expiry Notification Testing in Admin:**
  - In Admin Portal, check the **"1-Year Validity Expiry Alerts Hub"** to see pre-seeded accounts expiring soon. Click **"💬 Send WhatsApp Renewal"** or **"🔄 Renew 1-Year AMC"**.
- **Booking Capacity Test:**
  - Choose today's date in booking form. If 2 slots are already booked, the system automatically shows a capacity alert and disables booking for that date.
