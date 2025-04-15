# FlashDeal Browser Extension

FlashDeal is a browser extension that automatically finds and applies the best coupon codes when shopping online, helping users save money while generating revenue through affiliate marketing commissions.

## Project Overview

FlashDeal works by detecting when users are on checkout pages of supported online stores, then automatically testing various coupon codes to find the one that provides the biggest discount. The extension earns revenue through affiliate commissions when users make purchases using our tracked links.

### Website

Our official website is [myflashdeal.com](https://myflashdeal.com)

## Current Status

The project is in final development with:
- ✅ Complete extension functionality
- ✅ Fully implemented backend with Supabase database
- ✅ Landing page ready for deployment
- ✅ Affiliate integration strategy finalized
- ✅ Icon files and branding completed

Our target is to generate the first revenue within 12 hours of deployment.

## Project Structure

- `src/` - Frontend extension source code built with React
- `public/` - Static assets including icons and the manifest file
- `server/` - Backend API code using Express and Supabase
- `docs/` - Project documentation and guides

## Technology Stack

- Frontend: JavaScript, React
- Backend: Node.js, Express
- Database: Supabase
- Affiliate Management: Custom-built management system
- Deployment: Cloudflare Workers

## Getting Started

### Prerequisites

- Node.js (v16+)
- npm
- Supabase account (already set up at https://ksodvytwrkajdcjrtynf.supabase.co)
- Chrome browser for extension testing

### Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/flashdeal-extension.git
cd flashdeal-extension
```

2. Install dependencies:

```bash
npm install
```

3. Create a `.env` file in the server directory with your Supabase credentials:

```
SUPABASE_URL=https://ksodvytwrkajdcjrtynf.supabase.co
SUPABASE_ANON_KEY=your-anon-key
SUPABASE_SERVICE_KEY=your-service-key

# Affiliate network credentials
AMAZON_TRACKING_ID=flashdeal-20
SHAREASALE_AFFILIATE_ID=your-affiliate-id
CJ_PUBLISHER_ID=your-publisher-id
CJ_SITE_ID=your-site-id
```

4. Initialize the Supabase database:

```bash
cd server
node setup-supabase-fixed.js
```

5. Then run the SQL initialization script in Supabase SQL Editor (see `server/supabase-init.sql`)

6. Build the extension:

```bash
npm run build
```

### Development

Run the extension in development mode:

```bash
npm run dev
```

Run the server in development mode:

```bash
cd server
npm run dev
```

### Building for Production

Build the extension for production:

```bash
npm run build
```

The built extension will be in the `dist/` directory.

## Affiliate Network Integration

FlashDeal integrates with multiple affiliate networks to maximize revenue:

1. ShareASale/Awin (priority for 12-hour revenue goal)
2. Direct Merchant Programs (Walmart, eBay, Target)
3. CJ Affiliate
4. Rakuten Advertising
5. Amazon Associates (long-term revenue)

See the [Merchant Program Guide](./docs/MERCHANT_PROGRAM_GUIDE.md) for detailed instructions on applying to individual merchant programs within each network.

## Deployment

The extension is deployed in two parts:

1. The browser extension is published to the Chrome Web Store
2. The backend API is deployed to Cloudflare Workers
3. The landing page is deployed to myflashdeal.com

See the [Deployment Guide](./docs/DEPLOYMENT.md) for detailed deployment instructions.

## Revenue Strategy

Our approach to revenue generation is documented in [Affiliate Revenue Strategy](./docs/AFFILIATE_REVENUE_STRATEGY.md), which outlines how we prioritize different affiliate networks and merchant programs to maximize revenue in the shortest possible timeframe.

## Documentation

- [MCP_CHECKLIST.md](./MCP_CHECKLIST.md) - Complete implementation checklist
- [DEPLOYMENT.md](./DEPLOYMENT.md) - Deployment guide
- [AFFILIATE_SETUP_INDEX.md](./AFFILIATE_SETUP_INDEX.md) - Affiliate integration index
- [MERCHANT_PROGRAM_GUIDE.md](./docs/MERCHANT_PROGRAM_GUIDE.md) - Detailed guide for merchant program applications
- [AFFILIATE_REVENUE_STRATEGY.md](./docs/AFFILIATE_REVENUE_STRATEGY.md) - Strategy for maximizing affiliate revenue
- [SUPABASE_SETUP_GUIDE.md](./docs/SUPABASE_SETUP_GUIDE.md) - Guide for Supabase database setup

## License

This project is licensed under the MIT License - see the LICENSE file for details.
"# myflashdeal" 
