# 📘 DevOps Insiders – Detailed Notes
## Topic: **Time Management, Undivided Attention & 1-Tier Web Application Deployment**

---

## 1️⃣ Time Management & Undivided Attention

### 🔹 Core Principle

**“Ek baar me ek kaam” (Do one task at a time)**

Undivided attention means focusing completely on **one activity**, without distractions.

### ✅ Examples:

* 🍽️ **Eating Time** → Only eat (No Reels, No TV, No YouTube)
* 🧑‍💻 **Class Time** → Only class (No chatting, No multitasking)
* 🏢 **Office Time** → Only office work
* ⚽ **Playing Time** → Only play

### 🚶‍♂️ Health + Focus Rule

* **30–45 minutes daily walk**
* Improves:

  * Concentration
  * Mental clarity
  * Energy levels

👉 This habit is critical for **DevOps engineers**, because we handle:

* Servers
* Production systems
* Live deployments
  One mistake = downtime 🚨

---

## 2️⃣ Requirement Gathering (Product Company Example – GE)

### 🔹 What is Requirement Gathering?

Understanding:

* **What application already exists**
* **What we need to deploy**
* **Where it is hosted**
* **What tools/servers are required**

### 📌 Given Requirement:

* A **1-Tier Application** is **already developed**
* Code is stored on **GitHub**
* Application name: **StreamFlix**
* StreamFlix = **Netflix Clone Application**

👉 Our job is **deployment**, not development.

---

## 3️⃣ Understanding 1-Tier Architecture

### 🔹 What is a 1-Tier Application?

All components run on **a single machine**:

* UI (Frontend)
* Application Logic
* Data (if any)

### 🔹 In this case:

* Frontend code (HTML/CSS/JS)
* Web Server
* All hosted on **one server (Windows machine)**

### 📌 Used mostly for:

* Learning
* Demo projects
* Small websites

❌ Not suitable for large production systems

---

## 4️⃣ High-Level Architecture Explanation

### 🧑‍💻 Client–Server Concept

#### 🔹 Client:

* The one who **sends request**
* Examples:

  * Chrome
  * Firefox
  * Edge
  * Opera
* Client = **Browser**

#### 🔹 Server:

* The one who **listens to requests** and **responds**
* Example:

  * Web Server Software

📡 Flow:

```
Client (Browser) → Request → Server
Server → Response (HTML Page) → Client
```

---

## 5️⃣ What is a Web Server?

### 🔹 Definition:

A **Web Server** is a **software** that:

* Listens to browser requests
* Sends web pages (HTML, CSS, JS) as response

### 🔹 Example Response:

```html
Hello DevOps Insiders Community! We Love You!
```

### 🔹 Common Web Servers:

* IIS (Windows)
* Apache
* Nginx

---

## 6️⃣ Types of Servers (Conceptual Understanding)

* **Web Server** → Serves websites
* **Email Server** → Handles emails
* **FTP Server** → File transfer
* **SSH Server** → Secure remote access

Each server is **software**, not hardware.

---

## 7️⃣ Server vs Computer (Important Concept)

### 🔹 Hardware + Software = Computer

### 🔹 When a computer runs **server software**, it becomes a **server**

Example:

* Normal Computer + IIS = Web Server
* Normal Computer + FTP Service = FTP Server

👉 Server is defined by **role**, not machine.

---

## 8️⃣ IIS Web Server (Internet Information Services)

### 🔹 What is IIS?

* Microsoft’s **Web Server Software**
* Runs on **Windows OS**
* Used to host websites

### 🔹 Default Website Path:

```
C:\inetpub\wwwroot
```

Any file placed here becomes accessible via:

```
http://localhost
```

---

## 9️⃣ Installing IIS on Windows 11

### 🔹 How to Install:

* Google:

  ```
  How to install IIS on Windows 11
  ```
* Enable IIS from:

  * Windows Features
  * Turn Windows features ON/OFF

Once installed:

* IIS listens on port **80**
* Accessible via browser

---

## 🔟 Practical Deployment Steps (Recap)

### ✅ Steps Performed in Class:

1️⃣ Install **IIS** on Windows
2️⃣ Locate default path:

```
C:\inetpub\wwwroot
```

3️⃣ Delete default content (if required)
4️⃣ Download **Netflix Clone (StreamFlix)** code from GitHub
5️⃣ Extract ZIP file
6️⃣ Copy extracted files into:

```
C:\inetpub\wwwroot
```

7️⃣ Open browser and visit:

```
http://localhost
```

🎉 Result:
➡️ **Netflix-like website runs successfully**