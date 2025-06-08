# 🌐 Server

A social networking platform with automated content moderation and context-based authentication system — built with **Vibe Coding Cursor** and powered by a modern MERN stack.


---

## 📌 Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Technologies](#technologies)
- [Schema Diagram](#schema-diagram)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [License](#license)

---

## 🧠 Project Overview

**VibeTalks** is a full-stack social networking platform created using **Vibe Coding Cursor**. This project showcases not only advanced development skills but also deep integration of AI-driven moderation and security mechanisms.

Built with the **MERN (MongoDB, Express.js, React.js, Node.js)** stack, it includes:

- Automated **content moderation** using NLP APIs  
- **Context-based authentication** for secure logins  
- Classic social features like posts, likes, comments, follows  

### 🔍 Automated Content Moderation

Integrated APIs include:

- **Perspective API** – Detects toxicity, spam, harassment, etc.  
- **TextRazor API** – Categorizes content contextually  
- **Hugging Face Interface API** – Uses BART Large MNLI for zero-shot classification  

A custom **Flask-based classifier** using PyTorch replicates Hugging Face functionality for local deployment.

### 🔐 Context-Based Authentication

This system enhances user security using:

- IP, device & location data  
- AES encryption for secure storage  
- Email alerts for unusual login attempts  

---

## 🧑‍💼 User Roles

- **Admin** – Manages moderators, communities, content moderation  
- **Moderators** – Review flagged posts and manage communities  
- **Users** – Can post, comment, like, follow/unfollow others  

---

## ✅ Features

- 🔐 JWT-based user authentication  
- 👤 Profile and device management  
- 📝 Posting, commenting, liking  
- 📢 Reporting & moderation system  
- 🌍 Context-based login security  
- 📬 Email alerts for suspicious activity  
- 📊 Admin & Moderator Dashboards  

---

## 🛠 Technologies

- **Frontend**: React.js, Tailwind CSS, Redux  
- **Backend**: Node.js, Express.js, MongoDB  
- **Auth**: JWT, Passport.js, Crypto-js  
- **Email**: Nodemailer  
- **Storage**: Azure Blob Storage  
- **AI & Moderation**: Flask, Hugging Face Transformers  
- **Tools Used**: 🛠 Built using **Vibe Coding Cursor**

---

## 🗂 Schema Diagram

![Schema Diagram](https://raw.githubusercontent.com/nz-m/VibeTalks/main/resources/Schema-Diagram.png)

---

## 🚀 Getting Started

### 🔧 Prerequisites

- Node.js  
- MongoDB (local or Atlas)

### 📥 Installation

```bash
git clone https://github.com/nz-m/VibeTalks.git

Install dependencies:

```bash
cd client
npm install
```

```bash
cd server
npm install
```

Create `.env` files in `client/` and `server/` with relevant API keys (see `.env.example`).

### 🔌 Start the App

```bash
cd server
npm start
```

```bash
cd client
npm start
```

### ⚙️ Admin Setup

Run setup script:

```bash
./admin_tool.sh
```

### 🔐 Env Variables

For email alerts:

```env
EMAIL=
PASSWORD=
EMAIL_SERVICE=
```

For moderation:

```env
PERSPECTIVE_API_KEY=
INTERFACE_API_KEY=
TEXTRAZOR_API_KEY=
```

(You can also run the Flask-based classifier from `classifier_server/`.)

> ⚠️ Content moderation and auth features are optional but recommended for full functionality.

---

## 💻 Usage

### 👑 Admin

Visit `/admin` to access dashboard. You can:

- Create communities
- Manage moderators
- Toggle API services

### 🛡 Moderator

Register using `@mod.vibetalks.com` to auto-assign moderator role.

Moderators can review content & manage community discussions.

---

## 📜 License

Licensed under the [MIT License](https://github.com/nz-m/VibeTalks/blob/main/LICENSE).

---

## 🙋‍♂️ About Me

Hi! I'm **Manoj Kumawat**, a passionate developer and student from IIIT SURAT , Gujarat. I love building full-stack applications with creative ideas, and **VibeTalks** is one of my advanced MERN projects enhanced with **AI** and **security features**.


