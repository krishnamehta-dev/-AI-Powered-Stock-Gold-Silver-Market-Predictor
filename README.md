# Predicta

Predicta is a web-based market intelligence application built with Next.js and TypeScript. It provides market tracking, portfolio monitoring, price charts, and rule-based market signals for stocks, gold, and silver.

## Features

* Live market data from Yahoo Finance
* Stock tracking for NVIDIA, Apple, Tesla, and Microsoft
* Gold and silver market tracking
* Portfolio holdings management
* Portfolio value and profit/loss calculation
* Price charts and market trends
* Buy, Hold, and Watch signals
* Forecast price ranges
* Confidence scores for market signals
* Market data fallback for unavailable API data
* Responsive dashboard interface
* Database health check API

## Technologies Used

### Frontend

* Next.js
* React
* TypeScript
* Tailwind CSS

### Backend

* Next.js API Routes
* Node.js

### Database

* PostgreSQL
* Drizzle ORM

### Market Data

* Yahoo Finance API

## Supported Assets

### Stocks

* NVIDIA (NVDA)
* Apple (AAPL)
* Tesla (TSLA)
* Microsoft (MSFT)

### Gold

* Newmont (NEM)
* Barrick Gold (GOLD)
* SPDR Gold Shares (GLD)

### Silver

* iShares Silver Trust (SLV)

## Project Structure

```text
ai-stock-and-commodity-predictor/
|
├── src/
│   ├── app/
│   │   ├── api/
│   │   │   ├── health/
│   │   │   └── market/
│   │   ├── globals.css
│   │   ├── layout.tsx
│   │   └── page.tsx
│   │
│   ├── db/
│   │   ├── index.ts
│   │   └── schema.ts
│   │
│   └── lib/
│       └── market.ts
│
├── package.json
├── next.config.ts
├── tsconfig.json
├── eslint.config.mjs
├── postcss.config.mjs
└── drizzle.config.json
```

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/ai-stock-and-commodity-predictor.git
cd ai-stock-and-commodity-predictor
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure the database

Create a `.env.local` file and add:

```text
DATABASE_URL=your_postgresql_database_url
```

### 4. Start the development server

```bash
npm run dev
```

Open the application at:

```text
http://localhost:3000
```

## Available Commands

```bash
npm run dev
```

Starts the development server.

```bash
npm run build
```

Builds the application for production.

```bash
npm run start
```

Starts the production server.

```bash
npm run lint
```

Checks the project for linting issues.

```bash
npm run typecheck
```

Checks TypeScript types.

## How It Works

```text
User
  |
  v
Market Dashboard
  |
  v
Select Asset
  |
  v
Fetch Market Data
  |
  v
Analyze Price Movement
  |
  v
Generate Market Signal
  |
  v
Display Forecast and Chart
  |
  v
Track Portfolio
```

## Market Signal System

Predicta analyzes recent price movement and volatility to generate simple market signals.

```text
BUY
  |
Positive momentum

HOLD
  |
Balanced market movement

WATCH
  |
Negative or weakening momentum
```

The application also provides a confidence score and an estimated forecast range based on recent market data.

## Data Handling

The application first attempts to retrieve market data from Yahoo Finance.

If market data is unavailable, the application uses generated demo data so the dashboard can continue to operate.

## Future Improvements

* Machine learning based price prediction
* More stocks and commodities
* Historical performance analysis
* Advanced technical indicators
* User authentication
* Cloud portfolio storage
* Real-time price updates
* More detailed portfolio analytics
* Deployment to a production environment

## Developer

**Krishna Mehta**

Computer Science Undergraduate

Python | Machine Learning | Data Science | Web Development

## Project Highlights

Predicta combines modern web development with financial data analysis to create a focused market intelligence dashboard.

The project demonstrates experience with Next.js, TypeScript, API integration, PostgreSQL, data processing, portfolio calculations, and market analysis.

---

If you find the project useful, consider giving the repository a star.
