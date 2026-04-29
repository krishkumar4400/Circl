# 🚀 Circl — Full Project Documentation

**Resale Infrastructure Platform for D2C Brands (India)**

---

# 🧠 1. Executive Summary

## 📌 Product

**Circl** is a B2B SaaS platform that enables D2C brands to launch their own **“Certified Pre-Owned” resale ecosystem**.

## 🎯 Vision

Build the **resale infrastructure layer of India** powering circular commerce for brands.

## 💡 Core Idea

Brands currently lose value after first sale.
Circl enables them to **earn multiple times from the same product lifecycle**.

---

# 🔥 2. Problem Statement

## ❌ Customer Problems

* No trusted resale channel
* OLX = fraud risk, negotiation hassle
* Used products become dead assets

## ❌ Brand Problems

* One-time revenue per customer
* Returned/used inventory wasted
* No control over resale ecosystem
* Low customer retention

---

# 💥 Core Insight

> A single product can generate revenue multiple times — but brands lack the infrastructure to enable it.

---

# 💡 3. Solution

## 🧩 Circl Platform

A **white-label resale operating system** that allows brands to:

* Buy back used products from customers
* Refurbish and certify products
* Resell at discounted prices
* Track lifecycle and revenue

---

# 🔄 4. Product Workflow

```text
Customer → Sell Product → Brand Pickup → Refurbish → Relist → New Customer Buys
```

---

# 🧠 5. Key Features (INSANE VERSION)

## 🔥 5.1 Buyback Engine

* Customer submits product
* Instant price estimation
* Pickup scheduling

## 🤖 5.2 AI Pricing Engine

* Predict resale value based on:

  * Product age
  * Condition
  * Demand
  * Historical data

## 📸 5.3 Condition Detection (Future)

* Image upload
* AI detects wear & damage

## 🔄 5.4 Trade-in System

* Exchange old product for discount on new

## 📦 5.5 Inventory Management

* Track product lifecycle:

  * Received
  * Refurbishing
  * Ready
  * Sold

## 🔧 5.6 Refurbishment Workflow

* Assign repair tasks
* Quality checks
* Certification tagging

## 🛍️ 5.7 White-label Storefront

* Brand-specific resale website
* Custom branding

## 📊 5.8 Analytics Dashboard

* Revenue from resale
* Customer retention metrics
* Inventory insights

## 🚚 5.9 Logistics Integration

* Pickup & delivery
* Return handling

## 🔐 5.10 Trust System

* Certified Pre-Owned label
* Warranty options

---

# 💎 6. Unique Value Proposition

* Brand-controlled resale ecosystem
* Multi-revenue per product lifecycle
* AI-driven pricing & optimization
* Trust vs unverified marketplaces

---

# 🧠 7. Competitive Advantage (MOAT)

## 🔐 Data Moat

* Resale pricing database
* Product depreciation curves

## 🔄 Network Effects

* More brands → more products → more data → better pricing

## 🧱 Infrastructure Lock-in

* Logistics + refurb + pricing + dashboard

---

# 💰 8. Business Model

## 💵 Revenue Streams

| Type             | Description              |
| ---------------- | ------------------------ |
| SaaS Fee         | ₹10k–50k/month per brand |
| Commission       | 10–20% per transaction   |
| Logistics Margin | Pickup/delivery          |
| Refurbishment    | Service margin           |
| Data Insights    | Premium analytics        |

---

# 🎯 9. Target Market

## 🏢 Customers

* D2C brands (India)

## 📦 Categories

* Electronics
* Fashion
* Beauty
* Eyewear

---

# 🧱 10. System Architecture

```text
Frontend (Next.js)
    ↓
Backend API (Node.js / NestJS)
    ↓
Core Engine (Resale + Pricing + Workflow)
    ↓
Database (PostgreSQL)
    ↓
AI Layer (Pricing + Detection)
    ↓
External APIs (Payments, Logistics)
```

---

# 🛠️ 11. Tech Stack

## Frontend

* Next.js
* Tailwind CSS

## Backend

* Node.js (NestJS)

## Database

* PostgreSQL
* Redis

## AI

* OpenAI / custom ML
* Vector DB (optional)

## Infra

* AWS / Vercel
* S3 (images)

---

# 🗃️ 12. Database Schema

## Users

* id
* name
* email
* role

## Brands

* id
* name
* logo

## Products

* id
* brand_id
* name
* original_price

## ResaleItems

* id
* product_id
* condition
* status
* price

## Orders

* id
* buyer_id
* item_id
* status

## RefurbishmentTasks

* id
* item_id
* status

---

# 🔌 13. API Design

## Auth

* POST /auth/signup
* POST /auth/login

## Products

* GET /products
* POST /products

## Resale

* POST /resale/submit
* GET /resale/items

## Orders

* POST /orders
* GET /orders

---

# 🤖 14. AI System

## Pricing Model Inputs

* Original price
* Product age
* Condition
* Market demand

## Output

* Suggested resale price

---

# 🚀 15. MVP Plan

## Phase 1 (0–6 weeks)

* Single brand onboarding
* Buyback form
* Basic resale marketplace
* Manual pricing

## Phase 2

* Dashboard
* Payments
* Logistics

## Phase 3

* AI pricing
* Multi-brand system

---

# 🧲 16. Go-To-Market Strategy

## 🎯 Initial Focus

* 1 category (electronics)

## 📢 Acquisition

* LinkedIn outreach
* Founder connections

## 💡 Pitch

> “Increase your revenue by 20% using resale”

---

# 📊 17. Metrics

* GMV
* Revenue per brand
* Repeat purchases
* Inventory turnover

---

# ⚠️ 18. Risks

| Risk                 | Solution        |
| -------------------- | --------------- |
| Logistics complexity | API integration |
| Quality issues       | Strict QC       |
| Low adoption         | Start niche     |

---

# 🔁 19. Flywheel

```text
More brands → More resale → More data → Better pricing → More users → More brands
```

---

# 🏆 20. Long-Term Vision

* Become India’s resale infrastructure layer
* Expand to global markets
* Build sustainability intelligence platform

---

# 🔥 FINAL NOTE

Start simple.
Get 1 brand.
Generate ₹1.
Then scale.

---

## 🏗️ HIGH-LEVEL STRUCTURE (Monorepo + Microservices)

```
circl/
│
├── apps/                      # Frontend + public apps
│   ├── web-app/              # User (sell + buy)
│   ├── brand-dashboard/      # B2B dashboard
│   └── admin-panel/          # Internal ops
│
├── services/                 # Core backend microservices
│   ├── api-gateway/
│   ├── auth-service/
│   ├── user-service/
│   ├── product-ingestion-service/
│   ├── pricing-service/
│   ├── image-service/
│   ├── fraud-service/
│   ├── logistics-service/
│   ├── warehouse-service/
│   ├── inventory-service/
│   ├── listing-service/
│   ├── order-service/
│   ├── payment-service/
│   ├── notification-service/
│   └── analytics-service/
│
├── shared/                   # Shared libraries
│   ├── config/
│   ├── constants/
│   ├── utils/
│   ├── middleware/
│   └── types/
│
├── infra/                    # DevOps + infra
│   ├── docker/
│   ├── kubernetes/
│   ├── terraform/
│   └── ci-cd/
│
├── data/                     # Data pipelines & ML
│   ├── models/
│   ├── training/
│   ├── pipelines/
│   └── feature-store/
│
├── docs/                     # Architecture + APIs
│
└── scripts/                  # automation scripts
```

## 🔧 INSIDE A MICROSERVICE (Production Standard)

Example: pricing-service/

```
pricing-service/
│
├── src/
│   ├── controllers/
│   ├── services/
│   ├── repositories/
│   ├── models/
│   ├── routes/
│   ├── validators/
│   ├── middlewares/
│   ├── events/              # Kafka consumers/producers
│   ├── jobs/                # async jobs
│   ├── utils/
│   └── config/
│
├── tests/
│   ├── unit/
│   └── integration/
│
├── Dockerfile
├── package.json
└── README.md
```

🧠 CORE SERVICES BREAKDOWN
🔐 Auth Service
JWT / OAuth

role-based access

multi-tenant (brand-wise)

👤 User Service
user profiles

seller history

trust score

📦 Product Ingestion Service
upload product

metadata extraction

image upload

🤖 Pricing Service (CORE MOAT)
AI pricing

demand-based pricing

dynamic updates

🖼️ Image Service
compression

tagging

condition detection input

🚨 Fraud Service
fake detection

anomaly detection

🚚 Logistics Service
reverse pickup

delivery tracking

courier integration

🏭 Warehouse Service
QC

grading

refurb status

📊 Inventory Service
SKU management

stock lifecycle

🛍️ Listing Service
product listing

SEO + filters

🧾 Order Service
checkout

order lifecycle

💳 Payment Service
UPI / COD

refunds

🔔 Notification Service
email

SMS

WhatsApp

📈 Analytics Service
dashboards

data tracking


🧠 DATA LAYER (IMPORTANT)
Use hybrid:

PostgreSQL → transactions

MongoDB → flexible product data

Redis → caching

Elasticsearch → search

S3 → images

⚡ EVENT-DRIVEN FLOW
Use Kafka / queue:

User uploads product
   ↓
Event: PRODUCT_CREATED
   ↓
Pricing Service consumes
   ↓
Event: PRICE_GENERATED
   ↓
Listing Service consumes


☁️ INFRA STRUCTURE (AWS)
EKS (Kubernetes)

RDS (PostgreSQL)

S3 (images)

CloudFront (CDN)

SQS/Kafka

Redis (ElastiCache)

🧪 TESTING STRATEGY
unit tests (Jest)

integration tests

contract testing (API)

load testing


🔐 SECURITY
JWT auth

rate limiting

input validation

API gateway firewall

🚀 DEPLOYMENT FLOW
Code → GitHub
     ↓
CI/CD (GitHub Actions)
     ↓
Docker build
     ↓
Push to ECR
     ↓
Deploy to EKS

💡 IMPORTANT (FOUNDER LEVEL)
Krish, dhyaan se:

👉 Ye structure final nahi hai
👉 Ye starting scalable skeleton hai

⚠️ MVP VERSION (simplify)
Start with:

monolith backend (Node.js)

3 services only:

auth

product

order

👉 Phir gradually microservices me break kar

