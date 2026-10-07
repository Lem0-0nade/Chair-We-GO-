# Chair We GO! - Premium Event Rentals Web Application

Business Overview
* **Business Name:** Chair We GO!
* **Business Description:** Chair We GO! is a premier event rental service provider specializing in high-quality seating (monoblock chairs with optional fitted covers) and banquet/buffet tables. 
* **Target Users:** 
  * **Clients / Event Organizers:** Individuals or planners looking to reserve seating and tables for weddings, parties, corporate events, or private gatherings.
  * **Administrators:** Business owners/managers who oversee inventory capacities, track bookings on a live calendar, review client records, update payment statuses, and provide customer support.

Problem Being Solved
Traditional event equipment rentals often rely on manual spreadsheets, phone calls, or disjointed messaging apps to handle reservations, leading to double-booking errors, stock discrepancies, and delayed payment verifications. **Chair We GO!** solves this by providing an automated, real-time cloud concierge portal that locks inventory capacities instantly, prevents scheduling conflicts, calculates logistics (pick-up vs. delivery) dynamically, and unifies client-admin communication with image attachment support for proof-of-payment verification.

Feature List
* **Landing Page & Navigation**: Professional, artistic hero landing section with clear calls to action ("Reserve Now" and "Client Log In").
* **Authentication System**: 
  * User registration capturing Full Name, Email Address, and securely hashed passwords.
  * Flexible login using either **Email Address** or **Full Name**.
  * Secure session management and logout.
* **Role-Based Access Control**: Strict separation between Admin and regular User roles.
* **Complete CRUD Operations**:
  * **Create**: Register accounts, add new inventory stock capacities, and submit event reservations.
  * **Read**: Browse rental product catalogs, view client event histories, check event calendar schedules, and access chat support histories.
  * **Update**: Adjust cart item quantities, update stock inventory levels, and modify reservation payment statuses (e.g., marking payments as "Paid").
  * **Delete**: Remove items from cart or terminate/cancel event bookings (which automatically restores and frees up global inventory capacities).
* **Validations & Confirmations**: 
  * 4-day lead-time enforcement on reservation dates.
  * Real-time stock availability validation against global database records.
  * Confirmation dialogs before terminating reservations.
* **Flexible Logistics & Payments**: 
  * Selection between Store Pick-up (₱0) and Direct Delivery (₱300 with required address validation).
  * Choice of Cash payment or Online Payment via an integrated InstaPay QR code (revealed securely upon order confirmation).
* **Real-Time Client-Admin Support Chat & Attachments**: 
  * Live messaging widget with unread notifications.
  * Camera/file upload integration allowing clients to upload and transmit proof-of-payment screenshots directly to the admin.

Tech Stack Used
* **Frontend**: HTML5, CSS3 (Flexbox, CSS Grid, Custom Variables, Responsive Media Queries), Vanilla JavaScript (ES6+ Modules).
* **Database & Cloud Sync**: Firebase Realtime Database (Google Cloud).
* **Security**: Web Crypto API (SHA-256 Client-Side Password Hashing).

Setup and Run Instructions (Tested on Clean Machine)

1. **Clone the Repository**:
   ```bash
   git clone <your-repository-link>
   cd <repository-folder>
