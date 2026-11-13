<div align="center">

# 📊 YouTube Creator Analytics & Marketing Insights

### Find the *right* YouTube creators for your brand — using data, not guesswork.

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-Database-4479A1?logo=mysql&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-Analysis-orange)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black)
![YouTube API](https://img.shields.io/badge/YouTube%20Data%20API-v3-FF0000?logo=youtube&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)

</div>

---

## 📑 Table of Contents

1. [Dashboard Preview](#-dashboard-preview)
2. [What Is This Project?](#-what-is-this-project)
3. [The Business Problem](#-the-business-problem)
4. [How It Works](#-how-it-works)
5. [Tech Stack](#%EF%B8%8F-tech-stack)
6. [Repository Files](#-repository-files)
7. [What Gets Analyzed](#-what-gets-analyzed)
8. [Getting Started (Step by Step)](#-getting-started-step-by-step)
9. [Key Insights](#-key-insights)
10. [License & Author](#-license--author)

---

## 📸 Dashboard Preview

<p align="center">
  <img src="https://github.com/user-attachments/assets/a824db3f-0057-4767-a3d1-b4a7ecfee64e" alt="Dashboard Page 1" width="90%">
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/6f3eff04-1bc0-4698-8915-201a2df47331" alt="Dashboard Page 2" width="90%">
</p>

**Want to explore it yourself?**

| File | What it is |
|---|---|
| 📄 [`YoutubeAnalyticsDashboard.pdf`](YoutubeAnalyticsDashboard.pdf) | Printable snapshot of the dashboard. Open it in any PDF viewer. |
| 📈 [`YoutubeAnalyticsDashboard.pbix`](YoutubeAnalyticsDashboard.pbix) | The fully interactive Power BI file (needs Power BI Desktop). |
| 🎨 [`youtube_red.json`](youtube_red.json) | The custom **YouTube-red Power BI theme** that gives the dashboard its look and colors. |

---

## 🤔 What Is This Project?

This project collects real data from **10 YouTube channels**, stores it in a database, analyzes it with SQL, and shows the results in an interactive **Power BI dashboard**.

The goal: help a company decide **which YouTube creators are worth partnering with** by comparing their reach, engagement, and video performance side by side.

> 💡 **New to data analytics?** Think of it as a pipeline: *get data → store it → ask questions → show answers in charts.* That is exactly what this project does.

---

## 🎯 The Business Problem

An **EdTech startup** (a company that sells online courses) has **low course enrollments**. It wants to advertise through YouTube creators, but checking dozens of channels by hand is slow and unreliable.

This project answers questions like:

- 🌍 Which channels have the **biggest reach**?
- 💬 Which channels have the **most engaged audience**?
- 🎬 Which **videos perform best**?
- 🏷️ What **topics and tags** attract viewers?
- 📈 Which creators perform **consistently well**?
- ✅ Which creators are the **best fit** for a promotional campaign?

---

## 🔄 How It Works

```text
 ┌──────────────────┐     ┌─────────┐     ┌─────────┐     ┌──────────┐     ┌───────────┐
 │ YouTube Data API │ ──► │ Python  │ ──► │  MySQL  │ ──► │   SQL    │ ──► │ Power BI  │
 │       v3         │     │ (fetch) │     │ (store) │     │(analyze) │     │(visualize)│
 └──────────────────┘     └─────────┘     └─────────┘     └──────────┘     └───────────┘
                                                                                  │
                                                                                  ▼
                                                                  Recommended YouTube Creators
```

| Step | What happens |
|---|---|
| **1. Collect** | Python talks to the YouTube Data API and downloads channel + video details. |
| **2. Store** | The data is saved into MySQL tables so it is organized and searchable. |
| **3. Analyze** | SQL queries answer the business questions (top channels, best videos, etc.). |
| **4. Visualize** | Power BI turns the results into interactive charts and KPIs. |
| **5. Decide** | The company compares creators and shortlists the best partners. |

---

## 🛠️ Tech Stack

| Tool | Why it is used |
|---|---|
| 🐍 **Python** | Connects to the API and extracts the data automatically. |
| 📡 **YouTube Data API v3** | Official source of channel and video statistics. |
| 🗄️ **MySQL** | Stores all collected data in structured tables. |
| 🔍 **SQL** | Runs exploratory analysis to answer business questions. |
| 📊 **Power BI** | Builds the interactive dashboard and KPI visuals. |

---

## 📁 Repository Files

```text
YouTube-Creator-Analytics-Marketing-Insights/
│
├── 📓 Youtube_Analytics.ipynb          → Python notebook: fetch data from API & load into MySQL
├── 🔍 EDAYouTubeChannels.sql           → SQL queries for exploratory data analysis (EDA)
├── 📈 YoutubeAnalyticsDashboard.pbix   → Interactive Power BI dashboard
├── 📄 YoutubeAnalyticsDashboard.pdf    → PDF export of the dashboard
├── 🎨 youtube_red.json                 → Custom Power BI theme (YouTube red look)
├── 📜 LICENSE                          → MIT License
└── 📘 README.md                        → You are here!
```

---

## 🔍 What Gets Analyzed

| Area | What we look at |
|---|---|
| 📈 **Channel performance** | Subscribers, total views, number of videos, overall reach |
| 🎥 **Video performance** | Views, likes, comments, top-performing videos |
| 👥 **Audience engagement** | How actively viewers interact compared to channel size |
| 🏷️ **Content analysis** | Topics, keywords, and tags that attract viewers |
| ⚖️ **Channel comparison** | Side-by-side ranking of creators for campaign fit |

---

## 🚀 Getting Started (Step by Step)

### ✅ What you need first

- [Python 3.x](https://www.python.org/downloads/) and [Jupyter Notebook](https://jupyter.org/install)
- [MySQL Server](https://dev.mysql.com/downloads/mysql/)
- [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free, Windows)
- A **YouTube Data API v3 key** → [create one in Google Cloud Console](https://console.cloud.google.com/apis/library/youtube.googleapis.com)

### 🧭 Steps

**1️⃣ Download the project**

```bash
git clone https://github.com/DishantBhere/YouTube-Creator-Analytics-Marketing-Insights.git
cd YouTube-Creator-Analytics-Marketing-Insights
```

**2️⃣ Install the Python libraries**

```bash
pip install google-api-python-client pandas sqlalchemy pymysql jupyter
```

**3️⃣ Collect the data**

Open the notebook:

```bash
jupyter notebook Youtube_Analytics.ipynb
```

Add your **API key**, the **channel IDs** you want to study, and your **MySQL login**, then run all cells. The data will be saved into your MySQL database.

**4️⃣ Run the SQL analysis**

Open `EDAYouTubeChannels.sql` in MySQL Workbench (or any SQL tool) and run the queries.

**5️⃣ Open the dashboard**

1. Open `YoutubeAnalyticsDashboard.pbix` in Power BI Desktop.
2. Point it to your MySQL database and click **Refresh**.

**6️⃣ (Optional) Apply the custom theme to your own report**

1. In Power BI Desktop, go to **View → Themes → Browse for themes**.
2. Select `youtube_red.json`.
3. Your report now uses the YouTube-red color style.

> ⚠️ **Security tip:** Never upload your API key or database password to GitHub. Keep them in environment variables or a private config file.

---

## 💡 Key Insights

Picking creators by **subscriber count alone** can be misleading. This project combines several signals:

- ✅ High audience **reach**
- ✅ Strong **video performance**
- ✅ Better **engagement**
- ✅ **Relevant** content
- ✅ **Consistent** audience interest

Together they give a fairer, data-backed shortlist of creators for the EdTech campaign.

---

## 📜 License & Author

Released under the [MIT License](LICENSE).

**Built by [Dishant Bhere](https://github.com/DishantBhere)** — ⭐ star the repo if you found it useful!
