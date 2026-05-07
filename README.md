# 🎖️ Battalion Management System

<div align="center">

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Platform](https://img.shields.io/badge/platform-Base44-purple.svg)
![Status](https://img.shields.io/badge/status-Active-success.svg)

**A comprehensive military battalion management system for tracking soldiers, missions, daily reports, and manpower analytics.**

[Features](#-features) • [Architecture](#-architecture)  • [Usage](#-usage)

</div>

---

## 📋 Overview

The Battalion Management System is a full-stack web application designed to streamline military unit operations. It provides real-time tracking of soldier statuses, mission management, attendance reporting, and comprehensive analytics dashboards.

### Key Capabilities

- **Real-time Soldier Tracking** - Monitor soldier locations and statuses across multiple missions
- **Mission Management** - Create, edit, and manage missions with multiple locations
- **Daily Reporting (Report 1)** - Quick status updates with partial save functionality
- **Role-Based Access Control** - Granular permissions from platoon-level to global admin
- **Comprehensive Analytics** - Dashboards for manpower, attendance, and performance metrics
- **Multi-Location Support** - Assign companies and platoons to specific mission locations

---

## ✨ Features

### 👥 Soldier Management
- Complete soldier profiles with personal and military information
- Role-based categorization (Officer, Medic, Driver, etc.)
- Bulk import from Excel/CSV files
- Advanced search with debounce optimization
- Paginated results for large datasets

### 🎯 Mission Management
- Create missions with multiple locations
- Assign companies/platoons to specific locations
- Track mission duration and soldier participation
- Automatic status transitions

### 📊 Daily Status Reporting
- Quick grid-based status updates
- Partial save and resume capability
- Company-level progress tracking
- Historical report editing (admin approval required)
- Export to CSV

### 📈 Analytics Dashboards
- **General Dashboard** - Overall battalion status and trends
- **Manpower Dashboard** - Personnel statistics and distribution
- **Soldier History** - Individual soldier tracking over time

### 🔐 Role-Based Access Control (RBAC)
| Role | Permissions |
|------|-------------|
| Global Admin | Full system access, user management |
| Company Editor | Edit/view assigned company data |
| Company Viewer | View-only access to assigned company |
| Platoon Viewer | View-only access to assigned platoon |
| Global Viewer | Read-only access to all data |

### 📱 Additional Features
- Injury logging and tracking
- Commander reports and evaluations
- Reserve duty history
- Initial attendance reporting
- Absence tracking and alerts

---


## 🏗️ Architecture

### Tech Stack

| Layer | Technology |
|-------|------------|
| Frontend | React 18, Tailwind CSS, shadcn/ui |
| State Management | TanStack Query (React Query) |
| Backend | Base44 Platform (BaaS) |
| Database | Base44 Entities |
| Authentication | Base44 Auth |

### Project Structure

├── entities/ # Data models (JSON schemas) │ ├── Soldier.json │ ├── Mission.json │ ├── DailyStatus.json │ ├── Location.json │ └── ... │ ├── pages/ # Main application pages │ ├── Dashboard.js │ ├── Soldiers.js │ ├── Missions.js │ └── ... │ ├── components/ # Reusable components │ ├── soldiers/ │ ├── missions/ │ ├── status/ │ └── reports/ │ ├── functions/ # Backend functions │ ├── filterSoldiers.js │ └── sendAlert.js │ └── Layout.js

### ScreenShots


🔒 Security
Base44 authentication system
Row-Level Security (RLS) enforced
Role-based permissions on every request
📄 License
MIT License

Made with ❤️ for the IDF Reserve Forces

```
