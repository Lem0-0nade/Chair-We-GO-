# Chair We GO! - Premium Event Rentals Management System

## 1. Business Name & Description
* **Business Name:** Chair We GO!
* **Description:** Chair We GO! is a specialized event rental business providing high-quality monoblock chairs, round folding tables, and rectangular banquet tables for special occasions, parties, and gatherings. 
* **Target Users:** 
  * **Customers / Renters:** Individuals or event organizers looking to rent durable event seating and tables with transparent pricing, delivery management, and instant booking receipts.
  * **Business Owners / Administrators:** Store operators who need to manage inventory stock levels, monitor delivery logistics, track customer reservation history, and oversee a scheduling calendar.

---

## 2. Problem Being Solved
Before implementing this digital solution, event rental businesses typically faced several operational hurdles:
* **Double-Bookings & Stock Conflicts:** Manually tracking chair and table availability across multiple overlapping event dates often led to overbooking.
* **Lack of Advance Notice & Unreliable Bookings:** Last-minute "change-of-mind" bookings created logistical stress and preparation delays.
* **Ambiguous Delivery & Downpayment Terms:** Miscommunication regarding delivery distance fees and unconfirmed downpayments caused lost revenue.
* **Manual Record-Keeping:** Relying on paper ledgers or disorganized messaging apps for customer history, inventory tracking, and schedule validation.

**Chair We GO!** solves these problems by providing an automated, web-based platform with a mandatory 4-day advance booking window, dynamic distance-based delivery calculations, automatic 3-day downpayment tracking, and a centralized admin calendar.

---

## 3. Feature List
* **Public Landing Page:** A welcoming interface introducing the business value proposition, highlighting core features (Premium Quality, Fast Delivery, Easy Booking), and offering direct paths to log in or sign up.
* **User Authentication & Authorization:** Secure user registration and login system with persistent account memory (`localStorage`), featuring role-based redirection separating normal renters from store administrators.
* **Interactive Rental Catalog:** Displays item cards featuring high-resolution images, description cards with hover-zoom previews, and maximum stock limit visibility.
* **Advanced Reservation Cart:** 
  * Real-time subtotal calculation.
  * Combined direct number inputs and traditional `+` / `-` quantity buttons.
  * Venue address input and distance dropdown (+₱300 delivery fee if outside a 5km radius).
* **Professional Lead-Time Calendar Validation:** Restricts event booking dates to a minimum of **4 days in advance** from the current date to ensure adequate preparation time.
* **Policy Agreement & Automated Receipts:** Enforces a 50% downpayment policy within a 3-day window and generates printable/downloadable text receipts.
* **Comprehensive Admin CRUD Dashboard:**
  * **Inventory Management:** View real-time item capacities and dynamically update stock totals.
  * **Renter History Tracker:** View aggregate reservation counts and item breakdown history per customer.
  * **Interactive Schedule Calendar:** Visualizes daily bookings with status badges (*"Pending Downpayment"* vs. *"Paid"*), allowing administrators to mark payments or terminate/cancel unfulfilled bookings to automatically restore inventory stock.

---

## 4. Tech Stack Used
* **Frontend Structure:** HTML5 (Semantic markup, responsive grid layouts).
* **Styling & Presentation:** CSS3 (Custom CSS Variables, modern flexbox/grid alignments, smooth transition animations, and `@media` print stylesheet support).
* **Client-Side Logic & State Persistence:** Vanilla JavaScript (ES6+), utilizing browser `localStorage` to ensure data persists across page reloads and browser restarts without requiring an external backend database.
* **Hosting & Deployment:** Netlify (Static site drag-and-drop deployment).

---

## 5. Setup and Run Instructions (Tested from a Clean Machine)
Follow these steps to run the application locally or deploy it on a clean machine:

1. **Prepare the Project Directory:**
   Create a new folder on your computer named `chair-we-go`.
2. **Organize Assets:**
   Inside the `chair-we-go` folder, create a subfolder named `images`. Place your three item pictures inside this folder with these exact filenames:
   * `monoblock.jpg`
   * `round-table.jpg`
   * `rect-table.jpg`
3. **Add Application Code:**
   Save your complete HTML/JS application file into the root of the folder and name it **`index.html`**.
4. **Add Documentation:**
   Save this file as **`README.md`** inside the root folder.
5. **Run Locally:**
   * Double-click `index.html` to open it directly in any modern web browser (Google Chrome, Firefox, Microsoft Edge, Safari).
   * *Optional (Recommended for local web testing):* Open the folder in a code editor like Visual Studio Code and use the **Live Server** extension.

---

## 6. AI Tools Used & Purpose
* **AI Tool Utilized:** Gemini (Google AI Assistant)
* **Purpose & Contributions:**
  * **Full-Stack Application Development:** Assisted in architecting, writing, and iterating the single-file HTML/CSS/JavaScript application structure.
  * **Feature Integration:** Programmed complex business logic including the 4-day minimum lead-time restriction, distance-based delivery fee calculations (5km Morong radius rule), 3-day downpayment tracking, and interactive cart controls.
  * **Data Persistence Layer:** Configured `localStorage` handlers to seamlessly save user accounts, item inventories, and calendar schedules locally.
  * **UI/UX Enhancement:** Designed responsive cards with hover-zoom micro-interactions and sliding description reveals, alongside a professional landing page.
  * **Documentation:** Compiled technical deployment instructions and this structured project `README.md`.

---

## 7. Test Accounts & Sample Credentials
You can use the following default credentials to test both administrative and customer privileges immediately upon launching the system:

### Administrator Account
* **Role:** Store Manager / Admin Dashboard Access
* **Username:** `admin`
* **Password:** `admin`

### Sample Customer Account
* **Role:** Renter / Catalog & Cart Access
* **Username:** `Jane Doe` *(Or register a brand new account using the Sign Up page)*
* **Password:** `password123`
