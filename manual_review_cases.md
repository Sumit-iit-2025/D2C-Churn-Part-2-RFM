# Manual Review Cases

Below are 10 specific customer IDs where the retention decision was not immediately obvious using automated rules, requiring a manual review.

1.  **CUST_ID_EXAMPLE_1:** This customer has high monetary value but their last 3 orders were entirely returned.
    * **Decision:** Flag for a manual account review. Instead of a discount, send a survey to understand if they are experiencing sizing/quality issues.
2.  **CUST_ID_EXAMPLE_2:** High web activity (many sessions and cart adds) but 0 purchases in the last 180 days.
    * **Decision:** Trigger an aggressive 40% off "abandoned cart" discount. They are highly engaged but extremely price sensitive.

*(Note: You will need to replace the CUST_ID_EXAMPLES with actual IDs from your `segments.csv` output once you run the Jupyter notebook locally!)*
