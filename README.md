# QuantEdge AI Suite

Create a modern, premium, enterprise-grade responsive web application called "QuantEdge AI" – an AI-Powered Algorithmic Trading Platform.

The website should look like a real fintech SaaS product similar to Zerodha Streak, TradingView, or QuantConnect with a dark theme, glassmorphism UI, smooth animations, rounded cards, professional typography, and excellent spacing.

TECH STACK

- React + TypeScript

- Tailwind CSS

- Framer Motion

- Recharts

- React Router

- Responsive for Desktop, Tablet, and Mobile

THE WEBSITE MUST HAVE THE FOLLOWING PAGES

1. Landing Page

- Beautiful hero section

- Animated stock chart

- AI trading illustration

- CTA buttons

- Features

- Statistics

- Testimonials

- Pricing Plans

- FAQ

- Footer

2. Login

- Email login

- Password login

- Forgot password

- Social login UI

- Remember me

3. Register

- Full registration form

- Password strength

- Email verification UI

4. User Dashboard

Display:

- Total Portfolio Value

- Today's Profit/Loss

- Open Positions

- Available Balance

- Win Rate

- Active Strategies

- Market Overview Cards

- Portfolio Performance Chart

- Recent Trades

- Live Watchlist

- Notifications

5. Strategy Builder

Allow users to create trading strategies using:

- RSI

- MACD

- EMA

- SMA

- Bollinger Bands

- Volume

- ATR

- Supertrend

Each strategy should have:

- Entry Rules

- Exit Rules

- Stop Loss

- Target Profit

- Risk Percentage

- Timeframe

- Position Size

- Save Strategy

- Duplicate Strategy

- Delete Strategy

6. Backtesting Page

Features:

- Historical data simulation

- Equity Curve

- Profit Factor

- Maximum Drawdown

- CAGR

- Sharpe Ratio

- Win Rate

- Number of Trades

- Export Report

7. Live Trading

Display:

- Broker Connection

- Connected Status

- Active Orders

- Positions

- Auto Trading ON/OFF

- Emergency Stop Button

- Order History

8. Market Scanner

Filters:

- Price

- Volume

- RSI

- EMA Cross

- MACD

- Breakout

- Gap Up

- Gap Down

Display results in professional data tables.

9. AI Insights

Generate AI recommendations:

- Buy

- Sell

- Hold

- Risk Level

- Confidence Score

- Market Sentiment

- Sector Analysis

- News Summary

10. Portfolio Page

Display:

- Holdings

- Allocation Pie Chart

- Performance Graph

- Daily Returns

- Monthly Returns

- Annual Returns

- Dividend Summary

11. Reports

Generate:

- Monthly Reports

- Yearly Reports

- Tax Reports

- Trading Journal

- Export PDF

- Export Excel

12. Subscription Plans

- Free

- Pro

- Enterprise

Comparison Table

Payment Success Page

Payment Failed Page

13. Admin Panel

Dashboard:

- Total Users

- Active Users

- Revenue

- Strategies Created

- Trades Executed

- Server Health

- Subscription Analytics

Manage:

- Users

- Plans

- Strategies

- Payments

- Announcements

- Support Tickets

- Logs

- Roles & Permissions

14. Support Center

- Ticket System

- Live Chat UI

- Knowledge Base

- Contact Form

15. User Profile

- Personal Information

- Profile Photo

- Security Settings

- API Keys

- Two-Factor Authentication

- Notification Settings

- Activity Log

16. About Us

17. Contact Us

18. Privacy Policy

19. Terms & Conditions

20. 404 Page

DESIGN REQUIREMENTS

- Premium fintech dark UI

- Glassmorphism cards

- Professional gradients

- Smooth page transitions

- Hover animations

- Interactive charts

- Modern icons

- Sticky navigation

- Responsive layouts

- Clean dashboard

- Loading skeletons

- Toast notifications

- Empty states

- Error pages

DUMMY DATA

Populate every dashboard, chart, table, report, portfolio, and strategy with realistic sample trading data so the application appears fully functional without requiring a backend.

SPM PROJECT REQUIREMENTS

Structure the application as if it were a real software engineering project with clear modules, reusable components, scalable architecture, maintainable folder structure, proper routing, consistent UI design, and professional documentation comments in the code.

The website should look polished enough for a final-year university Software Project Management presentation.

This project was built with [Lovable](https://lovable.dev).

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/7bcfeb6b-7345-4fe0-8eb2-6bd5c84c1ad2).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js (v20+ or v22+) and npm:

```sh
git clone <this-repository-url>
cd <repository-name>
npm install
npm run dev
```

## Production Deployment to Vercel

This application is built with **TanStack Start** and **Nitro**, fully configured for deployment on **Vercel** with full support for Server-Side Rendering (SSR) and server APIs (`/api/market-data/*`).

### 1. Push Code to GitHub

```sh
git init
git add .
git commit -m "feat: production deployment readiness for Vercel"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo-name>.git
git push -u origin main
```

### 2. Import into Vercel

1. Log in to [Vercel Dashboard](https://vercel.com/dashboard).
2. Click **"Add New..."** -> **"Project"**.
3. Select your GitHub repository and click **Import**.
4. Configure the Project Settings:
   - **Framework Preset**: *Other* or *TanStack Start* (Vercel automatically detects the Nitro build output)
   - **Root Directory**: `./` (or `AlgoPlatfrom-main` if the subfolder was committed)
   - **Build Command**: `npm run build`
   - **Output Directory**: Automatically detected (`.vercel/output`)
   - **Install Command**: `npm install`
5. Configure **Environment Variables** (see below).
6. Click **Deploy**.

### 3. Environment Variables in Vercel

Under **Project Settings** -> **Environment Variables**, add the following variables:

| Variable Name | Required? | Description |
| :--- | :--- | :--- |
| `GROWW_API_KEY` | Optional | Groww API Developer Key (Required only for live Groww streaming ticks) |
| `GROWW_API_SECRET` | Optional | Groww API Secret Token (Required only for live Groww streaming ticks) |
| `DHAN_CLIENT_ID` | Optional | DhanHQ Client ID (Required only for live Dhan streaming ticks) |
| `DHAN_ACCESS_TOKEN` | Optional | DhanHQ Access/JWT Token (Required only for live Dhan streaming ticks) |
| `OTP_EXPIRY_SECONDS` | Optional | OTP expiration in seconds (Default: `60`) |
| `OTP_RESEND_COOLDOWN_SECONDS` | Optional | OTP resend cooldown in seconds (Default: `30`) |
| `OTP_MAX_ATTEMPTS` | Optional | Maximum OTP attempts (Default: `3`) |

*Note: If no broker credentials are provided, the application runs seamlessly in institutional mock / simulated paper-trading mode.*

