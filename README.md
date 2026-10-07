# Chair We GO! - Premium Event Rentals Web Application

**Chair We GO!** is a full-featured, responsive cloud web application built for event rental businesses. It streamlines inventory management, client authentication, event scheduling, dynamic logistics calculation, online/cash payments, and real-time client-admin support chat.

---

## 🚀 Key Features

* **Cloud-Synced Real-Time Database**: Powered by **Firebase Realtime Database**, allowing instant synchronization of inventory, bookings, user records, and chat messages across multiple devices and browsers.
* **Responsive Mobile & Desktop Web UI**: Fully optimized layout using advanced CSS media queries to ensure seamless viewing and usage on smartphones, tablets, and desktop computers.
* **Secure Client Authentication**:
  * Registration requires full name, email address, and a securely hashed password (SHA-256).
  * Flexible login supporting either **Email Address** or **Full Name**.
  * Hardcoded admin credentials removed from public views for enhanced security.
* **Interactive Event Rental Catalog**:
  * Real-time inventory tracking and stock counts.
  * Optional customized event additions (e.g., adding elegant fitted chair covers with dynamic pricing).
  * 4-day lead-time enforcement on reservation dates.
* **Flexible Logistics & Pricing**:
  * Choose between **Store Pick-up (₱0)** or **Direct-to-Venue Delivery (₱300)** with required address validation.
* **Dual Payment Modes & Online Verification**:
  * **Cash**: Pay upon pick-up or delivery.
  * **Online Payment**: Features an integrated InstaPay QR code displayed securely on the confirmation receipt *after* verification.
* **Proof of Payment Chat Attachments**:
  * Real-time chat widget enabling direct communication between clients and the admin.
  * Built-in camera/file upload button allowing clients to attach and send payment screenshots directly into the chat stream.
* **Interactive Event Calendar & Admin Dashboard**:
  * Monthly interactive event calendar tracking bookings and capacities.
  * Admin tools to update stock, monitor client histories, verify payment statuses, and terminate or manage bookings.
* **Digital Invoicing & Printing**: Generate, print, or download text-based formal invoices with full client details, item breakdowns, and billing totals.

---

## 🛠️ Technology Stack

* **Frontend**: HTML5, CSS3 (Custom Grid, Flexbox, Variables, Media Queries), Vanilla JavaScript (ES Modules).
* **Backend & Database**: Firebase Realtime Database (Google Cloud).
* **Security**: Web Crypto API (SHA-256 Hashing for passwords).

---

## ⚙️ Setup & Installation

1. **Clone or Download Files**: Ensure you have your `index.html` and the `images/` folder (containing your catalog images and `image_2b1985.png` InstaPay QR code) in your root directory.
2. **Firebase Configuration**: The project is pre-configured with a Firebase Realtime Database endpoint. Ensure your Firebase Database rules allow read/write access for testing:
   ```json
   {
     "rules": {
       ".read": "true",
       ".write": "true"
     }
   }
