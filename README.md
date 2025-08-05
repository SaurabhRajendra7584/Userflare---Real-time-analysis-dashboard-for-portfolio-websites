# 🚀 UserFlare: Real-Time Analytics Dashboard for Portfolio Websites

**UserFlare** is a live, real-time analytics solution built using **Google Analytics 4 (GA4)**, **Google Tag Manager (GTM)**, and **Looker Studio**, designed to monitor how users interact with a personal portfolio website. It tracks user behavior like page visits, button clicks, resume downloads, and more—helping you improve your site's performance with actionable insights.

---

## 📌 Project Highlights

- 📈 **Live Visitor Tracking** using GA4  
- 🎯 **Custom Event Tracking** (e.g., Resume downloads, Project clicks) via GTM  
- 📊 **Interactive Looker Studio Dashboard** with real-time visualizations  
- 🌐 **Free & Fully Web-Based** (Hosted on GitHub Pages or any static site)

---

## 🧰 Tech Stack

| Tool            | Purpose                                 |
|-----------------|------------------------------------------|
| GA4             | User session tracking and analytics      |
| GTM             | Event tagging without code changes       |
| Looker Studio   | Live dashboards and reporting            |
| GitHub Pages    | Hosting the portfolio site               |
| HTML/CSS/JS     | Basic structure for website integration  |

---

## 📂 Folder Structure

UserFlare/ ├── /website/           # Your portfolio site code (HTML/CSS/JS) ├── /dashboard/         # Screenshots or public link to Looker dashboard ├── README.md           # Project overview and setup guide

---

## ✅ Features Tracked

| Metric/Event                  | Description                                         |
|-------------------------------|-----------------------------------------------------|
| Page Views                    | Standard GA4 session data                           |
| Resume Download               | Custom GTM tag on resume file click                |
| Project Card Clicks           | Tracks user interest in showcased work             |
| Contact Form Submission       | Tracks lead generation intent                      |
| Scroll Depth                  | Detects how far users scroll on key pages          |
| Device/Location               | User tech and geo data via GA4                     |

---

## 🔧 Setup Instructions

### 1️⃣ Add GA4 to Your Website

1. Go to [Google Analytics](https://analytics.google.com/)
2. Create a **GA4 Property**
3. Add a **Web Stream** with your site URL
4. Copy the **Measurement ID** (e.g., `G-XXXXXXX`)
5. Use GTM to deploy this ID (see below)

---

### 2️⃣ Set Up Google Tag Manager (GTM)

1. Go to [Google Tag Manager](https://tagmanager.google.com/)
2. Create a new **Container** for your website
3. Copy the 2 GTM snippets and insert them:
   - `<head>` and `<body>` in your portfolio's HTML
4. Create a **GA4 Configuration Tag**
   - Add your GA4 Measurement ID
   - Trigger: All Pages

---

### 3️⃣ Add Custom Event Tags in GTM

#### 📄 Resume Download
- **Trigger Type:** Click → Link Click
- **Condition:** Click URL ends with `.pdf`
- **Event Name:** `resume_download`
- **GA4 Event Tag:** Linked to the GA4 Config tag

#### 💼 Project Card Clicks
- **Trigger Type:** Click on specific classes or IDs (`.project-card`)
- **Event Name:** `project_click`

#### 📬 Contact Submission
- **Trigger:** Form Submission or Button Click
- **Event Name:** `contact_submit`

Use GTM's Preview Mode to test all tags before publishing.

---

### 4️⃣ Build a Dashboard in Looker Studio

1. Go to [Looker Studio](https://lookerstudio.google.com/)
2. Connect your **GA4 property**
3. Add charts and filters like:
   - Line chart: Sessions Over Time
   - Scorecards: Total Users, Bounce Rate, Avg. Time
   - Table: Top Pages and Events
   - Pie Chart: Traffic Source Breakdown
   - Bar Chart: Events by Count (e.g., Resume Downloads)

4. Publish and embed or share your dashboard.

---

## 📸 Screenshots 
- here are some clicks from my project.
  
---

## 📈 Example Insights You Can Draw

- Which project gets the most clicks?
- How many visitors download your resume?
- Which countries and devices drive the most traffic?
- How far do users scroll on your homepage?

---

## 💡 Future Improvements

- Add heatmap integration using tools like Hotjar
- A/B test project layouts using GA4 experiments
- Track outbound links or blog reading patterns
- Push data to BigQuery for advanced querying

---

## 📜 License

This project is open-source and free to use under the MIT License.

---

## 🙌 Credits

Built with ❤️ by Saurabh Rajendra 
Hosted on GitHub Pages | Powered by GA4, GTM, Looker Studio

