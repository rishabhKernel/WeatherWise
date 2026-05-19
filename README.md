# ⛅ WeatherWise

🔗 **Live Deployment (AWS S3):**  
https://weatherwise-rishabh-app.s3-website.ap-south-1.amazonaws.com/

---

# 📌 Project Overview

WeatherWise is a sleek, responsive, and user-friendly weather web application designed to provide real-time weather information for any location worldwide.

This project was developed and deployed as part of the **AWS Cloud Assignment: “Deploying a Live Website on AWS Cloud Using EC2 or S3.”**

The application is fully hosted on **Amazon S3 Static Website Hosting** and is publicly accessible through a live URL.

The website uses the **OpenWeatherMap API** to fetch accurate live weather data based on:

- User’s current location
- Any searched city worldwide

---

# ☁️ AWS Cloud Deployment Details

## ✅ Deployment Platform
- Amazon S3 (Static Website Hosting)

## ✅ AWS Services Used
- Amazon S3
- S3 Static Website Hosting
- Bucket Policy Configuration
- Public Access Configuration

## ✅ Deployment Objectives Achieved
- Successfully created and configured an AWS S3 bucket
- Uploaded website source files to AWS Cloud
- Enabled static website hosting
- Configured bucket permissions for public access
- Generated a live public URL
- Successfully hosted the website online

---

# 🛠️ Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript (ES6+)
- AWS S3
- OpenWeatherMap API

---

# 🌟 Key Features

## 1️⃣ 📍 Location-Based Weather (Your Weather Tab)

- Uses the browser's **Geolocation API**
- Requests user permission to access coordinates
- Automatically fetches weather data for the current location
- Stores coordinates in `sessionStorage` for better user experience

---

## 2️⃣ 🔍 Search Weather by City

- Search weather for any city globally
- Fetches live weather data dynamically
- Displays accurate weather metrics instantly

---

## 3️⃣ 📊 Detailed Weather Information

The application displays:

- City Name
- Country Flag
- Weather Description
- Weather Icon
- Temperature (°C)
- Wind Speed (m/s)
- Humidity (%)
- Cloudiness (%)

---

## 4️⃣ 💫 User-Friendly Interface

- Responsive design for all devices
- Tab-based navigation
- Loading animation while fetching API data
- Smooth UI experience
- Basic error handling support

---

# 🧰 Technologies & APIs Used

## Frontend Technologies
- HTML5
- CSS3
- JavaScript (Vanilla JS)

## JavaScript Concepts Used
- DOM Manipulation
- Event Handling
- Async/Await
- Fetch API
- Geolocation API
- Session Storage API

## APIs Used
- OpenWeatherMap API
- FlagCDN API

---

# 📂 Project Structure

```bash
WeatherWise-main/
│
├── index.html
├── styles.css
├── index.js
├── images/
│   ├── cloud.png
│   ├── humidity.png
│   ├── loading.gif
│   ├── location.png
│   ├── search.png
│   └── wind.png
│
└── README.md
```

---

# 🚀 Steps Performed for AWS Deployment

## 1️⃣ Created an S3 Bucket
- Created a unique bucket in AWS S3
- Selected appropriate AWS region

## 2️⃣ Uploaded Website Files
- Uploaded HTML, CSS, JavaScript, and image assets

## 3️⃣ Enabled Static Website Hosting
- Enabled static website hosting in bucket properties
- Configured:
  - `index.html` as index document

## 4️⃣ Configured Public Access
- Disabled block public access settings
- Added bucket policy to allow public read access

## 5️⃣ Generated Live Website URL
- Successfully accessed the deployed website through AWS-generated endpoint

---

# 🔑 OpenWeatherMap API Key

The project currently uses an API key inside `index.js`.

```javascript
const API_KEY = "YOUR_API_KEY";
```

To use your own API key:

1. Create an account on OpenWeatherMap
2. Generate a free API key
3. Replace the existing API key in `index.js`

---

# 💻 How to Run Locally

## Clone Repository

```bash
git clone <repository-url>
```

## Open the Project

Simply open:

```bash
index.html
```

in any modern web browser.

You can also use:
- VS Code Live Server Extension

---

# 📚 Learning Outcomes

Through this project, I learned:

- AWS S3 static website deployment
- Cloud hosting fundamentals
- Website hosting configuration on AWS
- Bucket permissions and public access management
- Working with REST APIs
- Asynchronous JavaScript using async/await
- Browser Geolocation API
- Session Storage implementation
- Responsive UI development using CSS

---

# 📌 Assignment Objective Fulfilled

✔️ Developed a live website using web technologies  
✔️ Deployed the project on AWS Cloud  
✔️ Hosted website publicly using Amazon S3  
✔️ Generated a live accessible URL  
✔️ Understood cloud deployment workflow and hosting concepts  

---

# 👨‍💻 Developer

**Rishabh Chaurasia**
