# 📊 FinSight - Personal Finance Platform

**FinSight** is a cross-platform personal finance and budgeting application. It helps users track income and expenses, set budgets and savings goals, receive smart insights, and manage finances easily across web and mobile.

---

## 🚀 Features

- 📥 Manual and automated transaction tracking (SMS/Email/PDF)
- 📈 Budget and saving goal tracking
- 💡 Smart financial insights and alerts
- 🔔 Email, SMS, and push notifications
- 📄 PDF and CSV financial reports
- 🔐 Secure authentication with JWT
- 📱 React (Web) + React Native (Mobile)

---

## 🧱 Architecture

> Microservices-based architecture following domain-driven design.

| Service               | Responsibility                                |
|------------------------|-----------------------------------------------|
| `auth-service`        | Login, register, JWT token management         |
| `user-service`        | User profile and preferences                  |
| `transaction-service` | Expense/income tracking, auto-categorization |
| `account-service`     | Wallet, credit card, and bank tagging         |
| `budget-service`      | Monthly budget limits                         |
| `goal-service`        | Saving and investment goals                   |
| `insight-engine`      | Spending patterns and financial summaries     |
| `notification-service`| Push, Email, and SMS notification handling    |
| `parser-service`      | SMS, email, PDF parsing for transactions      |
| `report-service`      | PDF and CSV exports of financial data         |
| `config-service`      | Centralized configuration management          |
| `audit-service`       | Audit logs and history                        |
| `gateway`             | API routing, auth filters, rate limiting      |

---

## 📦 Tech Stack

- **Backend**: Java, Spring Boot, Spring Cloud, PostgreSQL, Kafka (future)
- **Frontend (Web)**: React + TypeScript
- **Frontend (Mobile)**: React Native (Expo)
- **CI/CD**: GitHub Actions, Docker
- **Infra (optional)**: Kubernetes, Helm, Terraform

---

## 🛠️ Getting Started

### 📁 Monorepo Folder Structure

```bash
FinSight/
├── auth-service/
├── user-service/
├── transaction-service/
├── ...
├── frontend/
│   ├── web/
│   └── mobile/
├── gateway/
├── config-service/
├── deploy/              # Docker-compose / Helm charts
├── .github/             # CI/CD workflows
└── README.md
