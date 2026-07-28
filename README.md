## Ata Hub - Landing Pages & Dynamic Booking Calendar

This Repository contains the front-end source code for Ata Hub (atahub.com), a local camera rental landing page serving students, creators, and photographers across Shah Alam, Klang, and Subang Jaya.

The goal of this website is to provide a smooth, conversion-focused user experience that handles gear browsing, add-on selections, live calendar availability checking, and direct WhatsApp bookings.

# Main Objectives & Features

* **Live Calendar Availability Sync:** Integrated directly a Google Sheet database CSV endpoint to parse real-time booking dates (start to return) and automatically update camera availability on the interactive calendar.

* **Frictionless Booking Flow:** Direct WhatsApp redirection populated with chosen camera details and specific dates for instant booking confirmation.

* **Gear Catalog & Add-Ons:** Displays main camera units (e.g., Canon EOS R50) alongside optional add-ons like extra batteries, tripods, and high-speed memory cards.

* **SEO & Local Business Schema:** Fully optimized with Structured Data (LocalBusiness JSON-LD), Open Graph metadata, and targeted local keywords for better search enging indexing.

* **Mobile-First & Performant:** Custom lightweight responsive design featuring scroll pop animations, modal views, touch-supported sliders, and no heavy UI frameworks.

# Tech Stack & Integrations
* **Frontend:** HTML5, Custom CSS3 (DM Sans & DM Serif Display fonts, CSS Variables, Flexbox/Grid), JavaScript (ES6+)

* **Data Source / Backend:** Google Sheets (Published CSV output for low-latency live booking queries)

* **Deployment & Hosting:** 

* **Third-Party Libraries:** FontAwesome 6 (Icons)

# Project Structure
.
├── index.html       # Landing page structure, schema, SEO tags, & modals
├── style.css        # Custom styles, responsive breakpoints, & pop animations
├── main.js          # Google Sheet CSV parser, modal handling, & calendar logic
├── images/          # Product assets, badges, & icons
└── README.md        # Project documentation

# How the Booking Sync Works

1. Booking entries (Camera, Start Date, Return Date) are logged in a Google Sheet workbook.

2. The sheet is published as a CSV endpoint.

3. main.js fetches and parses the raw CSV on page load, dynamically marking booked date ranges inside the modal calendar for each unit.

4. Unbooked days remain active and open WhatsApp with pre-filled messages specifying the date selected.

