# GluApp Server

**An advanced, secure, and real-time backend for comprehensive diabetes management.**

GluApp is an advanced diabetes management platform providing real-time glucose monitoring, health tracking, and CGM device integration. This repository contains the source code for the robust, scalable, and secure backend server that powers the GluApp ecosystem.

---

## About The Project

The GluApp server is the central nervous system of our platform, designed to provide a seamless and reliable experience for children, parents, and healthcare providers. It handles everything from real-time data ingestion from CGM devices to complex analytics and notifications, all while ensuring the highest standards of data security and privacy.

Our mission is to empower families and individuals managing diabetes by providing powerful, intuitive, and engaging tools. This server is the foundation of that mission.

---

## Key Features

The GluApp server is built with a focus on performance, reliability, and security. Here are some of the core features that make our platform stand out:

### 🚀 Blazing-Fast Real-Time Data Sync
* **WebSocket Integration**: Utilizes a high-performance WebSocket server for instantaneous, bidirectional communication between the app and the server.
* **Live Updates**: Glucose readings, alerts, and notifications are pushed to all connected family members and caregivers in real-time, ensuring everyone is always up-to-date.

### 🌐 Seamless CGM Integration
* **Multi-Provider Support**: Built-in, secure integrations with leading CGM providers, including **Dexcom (via OAuth2)** and **Abbott FreeStyle Libre (via LibreLinkUp)**.
* **Unified Data Model**: Consolidates data from various sources (CGM, manual entries, Nightscout) into a single, consistent format for reliable analysis.
* **Robust Sync Engine**: A dedicated service handles the fetching, transformation, and storage of CGM data, ensuring data integrity.

### 🧠 Intelligent Alerts & Notifications
* **Complex Alerting Engine**: A sophisticated `AlertService` evaluates incoming data against user-defined thresholds (high, low, rapid change) to generate timely and accurate alerts.
* **Multi-Channel Notifications**: Integrated with **Expo (Push)**, **Twilio (SMS & Voice)**, and **Mailjet/Nodemailer (Email)** to deliver critical alerts through the user's preferred channels.
* **Smart and Customizable**: Features include configurable quiet hours, alert snoozing, and an escalation system to notify emergency contacts.

### 📊 Powerful Data Analytics & Predictive Insights
* **Advanced Glucose Calculations**: Implements industry-standard calculations for metrics like Time-in-Range (TIR), eA1c, Standard Deviation, and Glucose Management Indicator (GMI).
* **Unified Trend Service**: A proprietary algorithm provides consistent and reliable trend analysis (e.g., `Rising`, `Falling`, `Stable`) across all data sources.
* **Pattern Recognition**: The `AnalyticsService` identifies recurring patterns like morning spikes or post-meal highs to provide actionable insights.

### 🎮 Engaging Gamification & Education for Children
* **Complete Gamification Engine**: Features a `GamificationService` and `HeroService` to manage XP, levels, ranks, quests, and achievements.
* **Interactive Learning**: The `EducationService` delivers structured lessons, activities, and quizzes tailored to different age groups, making diabetes education engaging and fun.
* **Hero Progression**: Children create and level up their own "hero" character by actively participating in their diabetes management, fostering a sense of accomplishment and ownership.

### 🔒 Secure & Private by Design
* **Robust Authentication**: Implements JWT-based authentication with access and refresh tokens, including token versioning to invalidate old sessions.
* **Data Encryption**: All sensitive data, such as third-party CGM provider tokens, is encrypted at rest using **AES-256-GCM**, the industry standard for strong encryption.
* **Privacy Controls**: A dedicated `PrivacySettings` model and API routes allow users to manage their data sharing and consent preferences.
* **Parental Controls**: A secure `parentPin` system protects sensitive actions and settings within the app.

---

## Getting Started

This is a private, proprietary codebase. For information on collaboration, partnerships, or investment opportunities, please reach out to our team.

## Contact

Project Lead - [hello@myglubear.com](mailto:hello@myglubear.com)

---
© 2025 GluBear. All Rights Reserved.
