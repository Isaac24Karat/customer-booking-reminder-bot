# Customer Booking Reminder Bot (n8n Workflow)

![Status](https://img.shields.io/badge/status-active-brightgreen)
![Built With](https://img.shields.io/badge/built%20with-n8n%20%7C%20Email%20%7C%20SMS-blue)
![Focus](https://img.shields.io/badge/feature-Automated%20Reminders-green)
![License](https://img.shields.io/badge/license-MIT-lightgrey)
![Last Update](https://img.shields.io/github/last-commit/Isaac24Karat/customer-booking-reminder-bot)


> **Project Pitch:**  
> I built a simple n8n workflow that monitors upcoming customer transfers and automatically sends reminders if the booking is within the next 24 hours.  
> This workflow helps improve customer communication, reduce missed pickups, and optimize operational efficiency.

---

## System Diagram

![Customer Booking Reminder Bot Diagram](customer-booking-reminder-diagram.png)

---

## What it Does
- Receives a list of bookings with transfer dates
- Checks if any booking is scheduled within the next 24 hours
- Sends an automated reminder notification for upcoming bookings
- Logs reminder actions for future reference

---

## Technologies Used
- **n8n** (workflow automation)
- **Webhook Node** (input trigger)
- **DateTime Comparison (Function Node)** (to calculate 24-hour windows)
- **Email Node** or **Set Node** (simulate reminder sending)
- **Set Node** (logging)

---

## Files
- **customer-booking-reminder-workflow.json** — Exported n8n workflow file
- **customer-booking-reminder-diagram.png** — Visual system diagram

---
## 📐 Reminder Personalization Logic
- Reminders adjust based on booking time + user timezone
- Can exclude return-trip reminders for one-way bookings


## Future Work

- Add support for SMS and push notification reminders
- Pull customer preferences from CRM for personalized timing
- Log missed pickups and retry logic
- Integrate with multilingual templates for broader customer support


---
*Demo built for AI Agent Implementation Manager portfolio presentation.*
