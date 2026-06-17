# Manual Review Cases

Below are 10 specific customer IDs pulled directly from the dataset where the retention decision was not immediately obvious using automated RFM rules, requiring a manual review.

## The "High-Spend, High-Return" Anomaly
These customers look like high-value VIPs based on monetary spend, but their return rates suggest a severe product or sizing issue.
1. **CUST00027:** Spent a massive ₹2,128.34 recently, but has a 100% return rate. 
   * **Decision:** Flag for manual account review. Do not send a discount. Instead, trigger a personalized email from Support asking if they need help with sizing or product matching.
2. **CUST00050:** Spent ₹2,026.54 with a 50% return rate. 
   * **Decision:** Similar to CUST00027, this indicates friction. Send a survey regarding product quality before they churn completely.

## The "Platinum but Furious" Anomaly
These customers hold the highest loyalty tier, but their recent interactions are extremely negative. Automated rules might falsely assume they are safe because of their Platinum status.
3. **CUST00074:** Platinum loyalty tier, but has a 100% negative sentiment rate on their recent support tickets.
   * **Decision:** Immediate phone call from a senior customer success manager. Platinum members with 100% negative sentiment are flight risks who can damage the brand reputation.
4. **CUST00413:** Platinum loyalty tier, also exhibiting a 100% negative ticket rate.
   * **Decision:** Manually review their ticket history to see if the issue was a systemic delivery failure. Issue a high-value store credit apology.

## The "High-Cart Abandonment, High-Spend" Anomaly
Standard rules say cart abandonment is a sign of churn risk, but these users contradict that.
5. **CUST00630:** Abandoned 5 carts in the last 30 days, yet still spent ₹1,967.63 recently. 
   * **Decision:** Do not send an abandoned cart discount. This user is clearly using the cart as a "wishlist" before making large bulk purchases. Giving them a discount would just erode our margin.
6. **CUST01985:** Abandoned 5 carts, spent ₹1,983.49. 
   * **Decision:** Same as above. Suppress them from automated abandoned cart promotional flows.

## The "Silent Churning Champions" Anomaly
These customers look perfect on paper but still churned.
7. **CUST00036:** Recency of 27 days, high frequency (4 orders), but the data shows they are a churn risk. They logged 1 recent support ticket.
   * **Decision:** The single support ticket might have been a catastrophic failure. Review the ticket transcript manually to understand why a top-tier champion would suddenly leave.
8. **CUST00184:** Recency of 14 days, Frequency of 3 orders. No support tickets logged.
   * **Decision:** This is a "silent churner." They may have switched to a competitor for reasons unrelated to our service (e.g., price). Send a "We Miss You - Tell Us How We Can Improve" survey.

## The "Severe Resolution Delay" Anomaly
These customers are high-value but suffered unacceptable wait times.
9. **CUST00053:** Spent ₹2,063.87, but their average support resolution time was a massive 56.1 hours.
   * **Decision:** Automatically upgrade their next 3 orders to expedited overnight shipping for free to apologize for the extreme delay.
10. **CUST00197:** Spent ₹2,989.16, but suffered a 54.3-hour resolution delay.
    * **Decision:** A customer spending nearly ₹3,000 should not wait 2+ days for an answer. Route them to a VIP support queue permanently.
