# Admin security notes
- Admin login is username + password. Only a salted SHA-256 hash is stored in js/data.js (ADMIN_AUTH).
- Session lasts 30 minutes, lives in sessionStorage, and ends when you leave the admin view or close the tab.
- Customer login/logout never grants or keeps admin access.
- LIMITATION: GitHub Pages is static hosting. This stops casual access, but a determined technical user can still
  read the page source. For real protection of customer data, move bookings/payments to a backend (Firebase Auth + Firestore).
