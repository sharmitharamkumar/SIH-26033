# Smart India Hackathon Workshop
# Date:28/10/2026
## Reference Number:26004703
## Name:Sharmitha R

## Problem Title
SIH 26033: Multiple intermediaries reduce farmers earnings and increase consumer prices.

## Problem Creater's Organization
Ministry of Consumer Affairs, Food & Public Distribution

## Theme
Agriculture, FoodTech & Rural Development

## Problem Description
Expected Solution: Create a digital marketplace that:

• Connects farmers/FPOs directly with consumers and bulk buyers.
• Provides logistics support.
• Uses AI for demand forecasting and route optimization.

Benefits:

• Better prices for farmers.
• Lower prices for consumers.
• Reduced supply chain inefficiencies.

## Proposed Solution

**Detailed explanation**

KisanLink is a digital marketplace that connects farmers and Farmer Producer Organizations (FPOs) directly with consumers and bulk buyers. Its key feature is that farmers can use it by voice, in their own language. A farmer sends a voice note or makes a call, such as "200 kg tomatoes, ready in two days." The system converts the speech to text and creates a product listing automatically. Buyers browse the listings on a web app, place orders and pay by UPI, and the money goes directly to the farmer. Produce is collected at a village hub and delivered using AI-planned routes.

**How it addresses the problem**

- Farmers sell directly, so the commission taken by middlemen is removed.
- The AI engine shows today's mandi price and a suggested fair price, so farmers are not underpaid.
- Demand forecasting tells farmers what buyers will need, which reduces unsold stock and wastage.
- Village hubs combine produce from many small farmers, making bulk delivery cheap.
- Consumers get fresher produce at lower prices because the supply chain is shorter.

**Innovation and uniqueness**

- Voice-first access in local languages, so farmers with low digital literacy can use it without learning an app.
- Village collection hubs that make logistics affordable for small and marginal farmers.
- One platform combining direct selling, AI price guidance, demand forecasting and route optimization.


## Technical Approach

**Technologies to be used**

- Farmer interface: WhatsApp voice notes and IVR phone calls
- Speech-to-text: Bhashini or OpenAI Whisper (supports Indian languages)
- Buyer interface: React web application
- Backend: Python (FastAPI) or Node.js
- Database: PostgreSQL
- AI/ML: Time-series forecasting (Prophet or LSTM) for demand and price prediction
- Route optimization: Google OR-Tools with Google Maps API
- Payments: UPI integration (e.g. Razorpay)
- Hosting: Cloud platform (AWS or Azure)

**Methodology and process for implementation**

1. The farmer sends a voice note or calls to list produce.
2. The speech-to-text module converts it into text in the local language.
3. The listing (crop, quantity, date) is stored in the database.
4. The AI engine suggests a fair price and forecasts demand.
5. The buyer browses the web app and places an order.
6. The buyer pays by UPI and the amount is credited directly to the farmer.
7. The route planner assigns pickup from the village hub and plans the delivery route.
8. The produce is delivered from the hub to the buyer.

## Feasibility and Viability
**Analysis of the feasibility of the idea**

The idea is realistic with existing tools. WhatsApp and UPI are already widely used in rural India. Speech-to-text for Indian languages is available through government and open-source platforms, and the AI components use proven libraries. A small pilot can start in one district with a few FPOs.

**Potential challenges and risks**

- Perishable produce can spoil during transport.
- Farmers may not trust a new platform.
- Rural internet connectivity can be weak.
- Last-mile delivery is costly.
- Speech recognition may struggle with local accents.

**Strategies for overcoming these challenges**

- Use village hubs with basic storage and fast pickup schedules.
- Work with trusted FPOs and local agriculture officers to build confidence.
- Offer IVR phone calls so the system works without internet.
- Combine many small orders at the hub to reduce delivery cost.
- Keep improving the speech model with local-language samples, and confirm each listing back to the farmer by voice.


## Impact and Benefits
**Potential impact on the target audience**

- Farmers: Higher income, faster payment and fair price information.
- Consumers: Fresher produce at lower prices.
- Bulk buyers and retailers: Reliable direct supply with transparent pricing.

**Benefits of the solution**

- Social: Includes farmers who are less educated or less tech-savvy, and strengthens FPOs and rural communities.
- Economic: Farmers keep a larger share of the final price, and value lost in the supply chain is reduced.
- Environmental: Demand forecasting reduces food waste, and optimized routes save fuel and cut emissions.


## Research and References
1. SIH 26033 problem statement, Ministry of Consumer Affairs, Food & Public Distribution
2. Agmarknet (mandi price data): https://agmarknet.gov.in
3. eNAM, National Agriculture Market: https://enam.gov.in
4. Bhashini, Government of India language platform: https://bhashini.gov.in
5. Google OR-Tools documentation (route optimization)
