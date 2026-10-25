# 🚗 Smart Road Alert Automation

An automated road incident alert system built using **n8n, Google Sheets, and Telegram**. This project processes road incident data, identifies high-priority alerts, and sends formatted notifications to Telegram.

## 📌 Project Overview

Smart Road Alert Automation aims to help drivers become aware of potential road incidents, heavy traffic, and road closures through automated notifications.

The workflow processes road incident records, filters alerts, prepares a summary, and sends the notification to a Telegram chat.

> **Note:** This project currently uses a sample dataset for demonstration. It does not yet receive live traffic or accident data.

## 🎯 Project Objectives

* Automate the processing of road incident data.
* Identify high-priority road alerts.
* Generate clear and informative alert summaries.
* Send notifications automatically through Telegram.
* Explore workflow automation using n8n.

## 🛠️ Technologies Used

* **n8n** — Workflow automation
* **Google Drive** — Sample dataset storage
* **Google Sheets** — Alert record management
* **Telegram Bot API** — Notification delivery
* **CSV** — Sample road incident dataset

## ⚙️ Workflow

1. **Schedule Trigger** — Starts the workflow at scheduled intervals.
2. **Search Files and Folders** — Locates the dataset in Google Drive.
3. **Download File** — Downloads the CSV dataset.
4. **Extract from File** — Extracts the road incident records.
5. **If** — Filters records according to the alert conditions.
6. **Code in JavaScript** — Processes the alert records.
7. **Google Sheets** — Stores alert information.
8. **Build Alert Summary** — Creates a readable alert message.
9. **Telegram** — Sends the alert notification.

## 📸 Project Screenshots

### 1. Workflow Overview

Shows the n8n workflow and the connections between its nodes.

![Workflow Overview](https://github.com/Savindi-Rathnayaka/Smart-Road-Alert-Automation/blob/main/Screenshot%202026-10-25%20184835.png)
![Workflow Overview](https://github.com/Savindi-Rathnayaka/Smart-Road-Alert-Automation/blob/main/Screenshot%202026-10-25%20184954.png)
### 2. Telegram Alert Notification

Example of the automated road incident alert message delivered to Telegram.

![Telegram Alert](https://github.com/Savindi-Rathnayaka/Smart-Road-Alert-Automation/blob/main/Screenshot%202026-10-25%20185126.png)


## 📊 Sample Dataset

The project uses a sample CSV dataset containing fields such as:

* `incident_id`
* `timestamp`
* `location`
* `incident_type`
* `severity`
* `distance_ahead_km`
* `current_speed_kmh`
* `free_flow_speed_kmh`
* `congestion_percent`
* `alert_required`
* `smart_alert_level`

The sample records represent different road conditions, including accidents, heavy traffic, and road closures.

## 🚨 Example Alert

```text
SMART ROAD ALERT

HIGH alerts: 684

Top 10:
Colombo - Baseline Road - Accident Reported
85.7% congestion, 5.7 km ahead

Please drive carefully!
```

The values above are based on the sample dataset and are provided for demonstration purposes only.

## 🔄 Automation

The workflow is configured to run at one-hour intervals using the n8n Schedule Trigger.

Automatic execution depends on the workflow being published and the n8n instance remaining available. The current sample dataset may produce repeated alerts because live data updates and complete duplicate-alert prevention have not yet been implemented.

## 🚀 Future Improvements

* Integrate a reliable real-time traffic or incident data source.
* Improve duplicate-alert prevention.
* Send alerts based on the driver's location.
* Add map-based incident visualization.
* Improve alert prioritization using traffic severity.
* Store and analyze historical road incident records.

## 👩‍💻 Author

**Savindi Rathnayaka**
(https://savindirathnayaka.app.n8n.cloud/assistant/ccf384fd-794e-4b0a-a12e-ab7ed3510a12)

Data Science Undergraduate | Interested in Data Analytics, Python, and Automation

