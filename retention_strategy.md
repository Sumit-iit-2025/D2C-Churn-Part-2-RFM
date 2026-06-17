# Retention Strategy & RFM Segments

## 1. Customer Segments Identified
Based on our dataset-backed RFM (Recency, Frequency, Monetary) calculations and support ticket history, we have segmented our customer base into the following five actionable cohorts:

**Segment 1: One-Time Buyer (Needs Onboarding)**
* **Behavior:** Customers who have only made exactly 1 purchase. Data shows this group has a severe 53.1% churn risk.
* **Retention Action:** Trigger an automated, mid-tier discount (16% - 26% off) specifically restricted to their second purchase. 
* **Expected Value:** Our EDA proves that getting a customer to cross the threshold into multiple purchases drops their churn rate down to 16.1%. Converting these users is the highest-leverage action the business can take.

**Segment 2: High-Value Unhappy**
* **Behavior:** Customers with high historical spend (Monetary > ₹1,000) who have logged 2 or more recent support tickets.
* **Retention Action:** Route immediately to a senior customer success agent for white-glove, manual outreach. Offer a "make-it-right" free replacement or high-value store credit rather than a standard percentage discount.
* **Expected Value:** Protects high-margin recurring revenue by neutralizing the friction of a poor customer service experience before the customer silently abandons the app.

**Segment 3: Champions (Safe)**
* **Behavior:** Highly active customers who purchased within the last 25 days and have made 3 or more total purchases. They exhibit a very low churn risk (~9.7%).
* **Retention Action:** Do NOT give margin-eroding discounts. Instead, offer retention through exclusivity: early access to new product launches or a free upgrade to the Platinum Loyalty Tier.
* **Expected Value:** Protects unit economics while increasing brand advocacy and lifetime value (LTV).

**Segment 4: Dormant (High Risk)**
* **Behavior:** Customers whose last purchase occurred over 129 days ago. Data shows an 89.2% probability of churning.
* **Retention Action:** Deploy a final, aggressive "win-back" campaign (e.g., 40% off or "Buy One Get One Free"). If they do not convert, suppress them from paid marketing channels to save ad spend.
* **Expected Value:** Cleans the active marketing list to improve ROI, while attempting to salvage a small percentage of near-lost accounts.

**Segment 5: Regular Active**
* **Behavior:** Standard repeat buyers who do not fit into the extreme risk or extreme champion categories.
* **Retention Action:** Maintain standard lifecycle marketing. Recommend products based on their `preferred_category` and engage them via standard email newsletters. 
* **Expected Value:** Maintains steady baseline revenue without unnecessary promotional costs.


## 2. Campaign Budget Prioritization
If given a limited campaign budget, I would prioritize the **One-Time Buyer (Needs Onboarding)** segment first, followed closely by the **High-Value Unhappy** segment. 

**Justification:**
1. Our EDA proved that the most critical drop-off point is the transition from the first to the second purchase. By spending promotional budget to secure that second purchase, we mathematically drop the customer's churn risk by roughly 37 absolute percentage points (from 53% to 16%). 
2. Furthermore, resolving the complaints of `High-Value Unhappy` customers is significantly cheaper than acquiring net-new customers who can spend over ₹1,000. 
3. We should actively *remove* budget from the `Champions` (who do not need discounts to buy) and the `Dormant` (who are likely a sunk cost), reallocating those funds to onboarding and VIP support.
