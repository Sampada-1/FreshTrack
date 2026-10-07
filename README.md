# FreshTrack

## Smart Expiry Management and Product Waste Reduction System

FreshTrack is a web-based product expiry management system designed to help users track product expiry dates, identify products that require attention, and make better decisions about usage, donation, and reuse.

The application provides multiple ways to add products, including image-based scanning, camera scanning, and manual entry. It calculates remaining shelf life and presents product information through an interactive dashboard with expiry insights, risk prioritization, analytics, notifications, donation support, and reuse suggestions.

## Features

* 🔐 **User Login Interface**
* 📷 **Product Image Scanning**
* 📸 **Camera-Based Product Scanning**
* ✍️ **Manual Product Entry**
* 🔎 **OCR-Based Date Extraction using Tesseract.js**
* 📅 **Expiry Date Tracking**
* ⏳ **Days Remaining Calculation**
* 🟢 **Product Status Classification**
* 🤖 **Rule-Based Expiry Risk Prioritization**
* 📊 **Interactive Dashboard**
* 📈 **Inventory Health Visualization**
* 🗓️ **Interactive Expiry Timeline**
* 🔍 **Product Search, Filtering and Sorting**
* 📄 **CSV Expiry Intelligence Report Export**
* 🔔 **Expiry Notifications**
* 🎁 **Donation Management**
* 🤝 **Donation Interest/Request Workflow**
* ♻️ **Product Reuse Suggestions**
* 📦 **Inventory Management**
* 📊 **Product Demand and Trend Information**
* 📱 **Responsive User Interface**

## Smart Expiry Risk Analysis

FreshTrack includes a rule-based risk analysis layer that evaluates products according to their expiry proximity.

The current implementation classifies products into:

* **Low Risk** – more than 7 days remaining
* **Medium Risk** – 4–7 days remaining
* **High Risk** – 0–3 days remaining
* **Expired** – expiry date has passed

The system also generates recommendations based on the calculated expiry risk.

> **Note:** The current "AI Risk" feature is a rule-based local prediction system. It is not a trained machine-learning model or a food-safety certification system.

## Product Scanning

FreshTrack supports different product-input methods:

1. **Image Upload** – upload a product/date-label image.
2. **Camera Scan** – capture the product label using the camera.
3. **Manual Entry** – enter product information manually.

OCR functionality is implemented using **Tesseract.js** to assist with extracting information from product labels.

## Dashboard

The FreshTrack dashboard provides an overview of the tracked inventory, including:

* Total products
* Safe products
* Products expiring soon
* Expired products
* Donation-priority products
* Inventory health
* Risk priorities
* Waste risk
* Urgent items
* Recommended actions
* Expiry timeline

Users can also search, filter, sort, refresh the dashboard, and export an expiry intelligence report.

## Donation Management

Products approaching expiry can be considered for donation where appropriate.

The donation module allows users to provide information such as:

* Product name
* Quantity
* Expiry date
* Product description
* Donor/contact information

The system also provides a workflow for users interested in available donations.

## Reuse Suggestions

FreshTrack provides reuse ideas for selected product categories to encourage responsible use and reduce unnecessary waste.

The reuse section includes categorized suggestions and filtering options.

## Analytics and Demand Information

The application includes product demand and trend information using a built-in product dataset.

Users can search for products and view information such as:

* Product category
* Demand level
* Demand trend
* Available brands

## Notifications

FreshTrack provides expiry-related notification functionality to help users identify products that need attention.

The current implementation is a **frontend/demo notification system** using browser-side storage and local processing.

For production-level cross-device notifications, a backend notification service would be required.

## Technologies Used

* **HTML5**
* **CSS3**
* **JavaScript**
* **Tesseract.js**
* **Chart.js**
* **Browser Local Storage**
* **Browser Session Storage**
* **CSV Export**

## Project Structure

The current project is intentionally maintained as a single-page application:

```text
FreshTrack/
│
├── index.html
└── README.md
```

The `index.html` file contains the complete FreshTrack application, including its HTML structure, CSS styling, and JavaScript functionality.

## How to Run

### Option 1 — Open Directly

1. Download or clone this repository.
2. Open the project folder.
3. Double-click `index.html`.
4. FreshTrack will open in your web browser.

### Option 2 — Using VS Code

1. Open the `FreshTrack` folder in Visual Studio Code.
2. Open `index.html`.
3. Run the file using a browser or a local development extension such as Live Server.

## Project Objective

The main objective of FreshTrack is to provide a simple digital solution for monitoring product expiry, prioritizing products that need attention, supporting responsible donation and reuse, and helping reduce avoidable product waste.

## Current Limitations

* Authentication is currently implemented as a frontend/demo interface.
* Product and application data are stored locally in the browser.
* The risk analysis is rule-based rather than a trained ML model.
* Cross-device synchronization requires a backend.
* Production-grade notification services would require backend integration.

## Future Enhancements

* 🤖 Machine-learning-based expiry prediction
* ☁️ Cloud database and synchronization
* 🔐 Backend authentication and authorization
* 📱 Mobile application
* 🔔 Real-time push notifications
* 📊 Advanced predictive analytics
* 🧠 Demand forecasting
* 🌐 Multi-user cloud support
* 🏷️ Improved product-label and barcode recognition

## Project

**Project Name:** FreshTrack
**Type:** Web-Based Smart Expiry Management System
**Domain:** Product Expiry Management, Waste Reduction and Smart Analytics

---

⭐ If you find this project useful, feel free to explore the repository and the implementation.
