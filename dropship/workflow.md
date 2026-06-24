# 🚚 Dropship Pipeline: 1688 → Shopee → TikTok Shop

> Compiled from YouTube tutorials (Jun 2026). This is the MANUAL process.
> Automation target: replicate every step using Nanobrowser + DeepSeek V4 Flash.

---

## 📦 PHASE 1: Find Products on 1688 (Source)

### 1.1 Access 1688
- Open 1688.com (Chinese B2B marketplace)
- Translate page to English (browser auto-translate)
- Log in with account (register via phone number if needed)

### 1.2 Search & Select Products
- Search for product category (e.g. "phone case", "slippers", "toys")
- Look for products with:
  - ✅ Multiple color/size variants
  - ✅ Detailed product parameters (dimensions, material, weight)
  - ✅ User reviews with photos
  - ✅ Merchant willing to do dropshipping (contact to confirm)

### 1.3 Extract Product Data
- **Copy product title** (original Chinese + English translation)
- **Copy product description** (specifications, features, materials)
- **Download product images** (at least 3-5 high quality photos)
- **Record price & variants** (colors, sizes, quantities)
- **Save user reviews** (proof of quality)
- **Contact merchant** to negotiate dropship terms:
  - Can they ship directly to customer?
  - What are shipping costs (international)?
  - Do they offer tracking numbers?
  - Payment terms?

---

## 🛒 PHASE 2: List on Shopee

### 2.1 Prerequisites
- Shopee seller account (register if needed)
  - Business information required: tax info, business registration, VAT/TIN
  - Personal or business account
- CJ Dropshipping account (connector) — OR negotiate directly with 1688 supplier

### 2.2 Connect Dropship Source (CJ Method)
- Log into CJ Dropshipping
- Connect to Shopee store (integration settings)
- Authorize CJ to push products to Shopee

### 2.3 Create Product Listing (Manual Method)
- Go to Shopee Seller Center → Add New Product
- **Upload images**: minimum 3 images (product photos from 1688)
- **Set product name**: translate/copy from 1688
- **Select category**: match product type on Shopee
- **Set product description**: copy specs, features, materials from 1688
- **Set sales info**: price (cost from 1688 + markup + shipping), variants (color/size)
- **Set shipping**: configure shipping template (domestic MY or international)
- **Save & Publish**

### 2.4 Order Fulfillment (When Customer Buys)
- Customer places order on Shopee
- Copy customer's shipping address & order details
- Send delivery info to 1688 supplier / agent
- Supplier ships directly to customer
- Supplier provides tracking number
- Update Shopee with tracking info
- Agent can provide Excel tracking sheet for bulk orders

---

## 🎵 PHASE 3: List on TikTok Shop

### 3.1 Prerequisites
- TikTok Shop seller account (register at shop.tiktok.com)
- Options: Individual (no business reg) or Sole Proprietorship (with LLC)
- Required: ID upload, tax info (SSN/TIN), address verification
- Wait for approval (hours to 1 day)

### 3.2 Configure Shipping (Critical!)
- **Fulfillment Settings** → Add Warehouse
  - Name your warehouse (e.g. "MY Warehouse")
  - Add contact info (can use virtual address)
  - Remove Hawaii & Alaska from shipping zones
- **Shipping & Delivery** → Select Seller Shipping (NOT TikTok shipping)
  - Create shipping template:
    - "Standard" delivery (7 business days) — recommended
    - Flat rate: $0 (free shipping → build cost into product price)
    - Avoid "Express" (4 days — too tight for dropship)
    - Avoid "Free Economy" (11 days — deters customers)

### 3.3 Find Winning Products
- **Method A: Product Research Tools** (AutoDS recommended)
  - 30-day trial for $1
  - Trending Products tab: filter by likes, impressions, engagement
  - Check Amazon Prime availability (must have fast shipping!)
  - Check existing TikTok Shop competitors already making sales
- **Method B: Manual scrolling**
  - Browse TikTok Shop, Amazon best sellers
  - Look for products with existing viral videos you can replicate
- **Product criteria:**
  - ✅ Amazon Prime listing available (2-day shipping) — CRITICAL
  - ✅ You fit the target demographic (or can replicate competitor videos)
  - ✅ Already going viral for 2+ other sellers (proof of concept)
  - ✅ Not restricted by TikTok policies

### 3.4 Create Product Listing
- Go to Products → Add New Product
- **Upload images** (from 1688 or supplier)
- **Product name**: clear, keyword-optimized
- **Category**: select matching category
- **Description**: from 1688 product specs
- **Price**: cost + markup (factor in shipping cost)
- **Connect supplier for fulfillment**:
  - Option A: AutoDS automation (auto-order from Amazon on customer purchase)
  - Option B: Manual fulfillment via Amazon Prime
  - Option C: Supplier direct (if they can do fast shipping)

### 3.5 Content Creation (Drives Traffic)
- **Method 1: Record yourself**
  - Order product to your house (return within 30 days if needed)
  - Record unboxing, demo, lifestyle shots
  - No need to show face or speak! (masks, POV, B-roll work)
- **Method 2: AI-generated videos** (Create UGC, etc.)
  - Paste Amazon/1688 listing link → AI generates video with avatar
  - Or generate attention-grabbing hooks (AI) + real clips (hybrid)
- **Method 3: Copy competitors' format**
  - Find what's working → recreate with your own footage

### 3.6 Drive Sales
- Post content on TikTok account linked to your Shop
- Use TikTok's built-in Affiliate Program:
  - Creators promote your product for commission (you only pay per sale)
  - Set commission percentage
  - Approve creators or open to all
- Run flash sales (create urgency without cutting price)
- Post consistently — scale with creators who do the posting for you

### 3.7 Order Fulfillment
- AutoDS automation (recommended):
  - Connect TikTok Shop → AutoDS → Amazon listing
  - When customer orders, AutoDS auto-places order on Amazon
  - Amazon ships directly to customer
  - Tracking auto-updates in TikTok Shop
- OR Manual: copy customer info → order from Amazon/1688 supplier → paste tracking

---

## 🔄 PHASE 4: Full Pipeline Automation (With Nanobrowser)

### Step-by-step automation tasks:

```
STEP 1: Login & Navigate
  ├── Open 1688.com, log in
  ├── Open Shopee Seller Center, log in
  └── Open TikTok Shop Seller, log in

STEP 2: Scrape 1688 Product
  ├── Navigate to product page
  ├── Save title, description, specs, images
  ├── Save price, variants, stock info
  └── Save user reviews

STEP 3: Create Shopee Listing
  ├── Click "Add New Product"
  ├── Upload images (from STEP 2)
  ├── Fill title, category, description
  ├── Set price (cost + markup)
  ├── Set variants (color, size, stock)
  ├── Configure shipping template
  └── Click "Save & Publish"

STEP 4: Create TikTok Shop Listing
  ├── Click "Add Product"
  ├── Upload images (from STEP 2)
  ├── Fill product details
  ├── Set price with free shipping
  ├── Connect to fulfillment (AutoDS or Amazon Prime link)
  └── Click "Save & Publish"

STEP 5: Content Generation
  ├── Download product images from 1688
  ├── Optional: Process via ComfyUI (resize, background removal)
  ├── Generate video ideas from competitor analysis
  └── Post to TikTok account

STEP 6: Monitor & Fulfill
  ├── Check Shopee for new orders (daily)
  ├── Check TikTok Shop for new orders (daily)
  ├── Send fulfillment info to supplier
  └── Update tracking numbers
```

### Automation Triggers (Schedule)
- **Daily at 08:00** — Check for new orders on Shopee + TikTok
- **Every 6 hours** — Search 1688 for trending products matching keywords
- **Weekly** — Post new content to TikTok
- **On-demand** — List a new product on both platforms

---

## 🛠 Tech Stack for Automation

| Tool | Role | Cost |
|---|---|---|
| **Nanobrowser** (Chrome extension) | Vision-based browser automation in your real Chrome | Free |
| **DeepSeek V4 Flash** | AI brain — sees screenshots, decides clicks | Your API key (pay-per-token) |
| **ComfyUI** (optional) | Image processing (resize, background removal, enhancement) | Free (WSL) |
| **AI Surfer OS Dashboard** | Monitoring, scheduling, pipeline status | Already running (:3333) |
| **AutoDS** (optional) | Product research + auto-fulfillment via Amazon | $1/30 days trial |
| **Amazon Prime** | Fulfillment source for TikTok Shop (must have) | Per-order cost |

## 📋 Key Rules from Tutorials

1. **TikTok Shop: MUST use Amazon Prime** — TikTok requires delivery within 6 business days. 1688 direct shipping is too slow. Use Amazon as fulfillment middle-man.
2. **1688 → Shopee: Use CJ Dropshipping** as connector for automatic order forwarding.
3. **Markup rule**: Product cost + shipping cost + at least 30% margin = your selling price.
4. **Shopee requires business registration** — tax info, VAT/TIN, business entity docs.
5. **TikTok Shop: individual accounts work** — no LLC needed to start (just ID + tax number).
6. **Product criteria for TikTok**: Must be trending / already viral for 2+ sellers. Don't invent new products — copy what works.
