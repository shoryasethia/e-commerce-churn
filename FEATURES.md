| **Feature Name**                        | **Category**            | **Abbreviated Name** | **Definition**                                                                                       |
|-----------------------------------------|-------------------------|----------------------|-------------------------------------------------------------------------------------------------------|
| Session Recency                         | Recency                 | `ses_rec`            | Days between last user session and reference date                                                     |
| Average Session Recency                 | Recency                 | `ses_rec_avg`        | Average days between consecutive sessions                                                              |
| Session Recency Standard Deviation      | Recency                 | `ses_rec_sd`         | Standard deviation of time between sessions (days)                                                    |
| Session Recency Coefficient of Variation| Recency                 | `ses_rec_cv`         | Ratio of std dev to mean time between sessions (%)                                                    |
| User Maturity                           | Recency                 | `user_rec`           | Days since user's first session                                                                       |
| Session Count                           | Frequency               | `ses_n`              | Total number of sessions                                                                               |
| Relative Session Frequency              | Frequency               | `ses_n_r`            | Sessions per day since first activity                                                                 |
| Interaction Count                       | Frequency               | `int_n`              | Total number of events (view/cart/purchase)                                                            |
| View Count                              | Frequency               | `view_count`         | Total number of view events                                                                            |
| Cart Count                              | Frequency               | `cart_count`         | Total number of cart events                                                                            |
| Purchase Count                          | Frequency               | `purchase_count`     | Total number of purchase events                                                                        |
| Interaction Rate                        | Frequency               | `int_n_r`            | Average interactions per session                                                                       |
| Transaction Count                       | Frequency               | `tran_n`             | Total number of transactions (purchases)                                                              |
| Transaction Rate                        | Frequency               | `tran_n_r`           | Average transactions per session                                                                       |
| Total Revenue                           | Monetary                | `rev_sum`            | Total spending by user (USD)                                                                           |
| Average Purchase Value                  | Monetary                | `rev_per_purchase`   | Average amount spent per purchase                                                                      |
| Revenue per Session                     | Monetary                | `rev_sum_r`          | Average revenue per session                                                                            |
| High Spender Flag                       | Monetary                | `major_spend_r`      | Whether user's spending is above average (1/0)                                                         |
| Category Interaction Count              | Category & Item         | `int_cat_n`          | Number of unique categories interacted with                                                             |
| Product Interaction Count               | Category & Item         | `int_itm_n`          | Number of unique products interacted with                                                               |
| Category Diversity                      | Category & Item         | `int_cat_n_avg`      | Average unique categories per session                                                                   |
| Product Diversity                       | Category & Item         | `int_itm_n_avg`      | Average unique products per session                                                                     |
| Average Month                           | Date & Time             | `ses_mo_avg`         | Average month of user sessions (1-12)                                                                  |
| Month Standard Deviation                | Date & Time             | `ses_mo_sd`          | Variation in session months                                                                             |
| Average Hour                            | Date & Time             | `ses_hr_avg`         | Average hour of day for sessions (0-23)                                                                |
| Hour Standard Deviation                 | Date & Time             | `ses_hr_sd`          | Variation in session hours                                                                              |
| Weekend Ratio                           | Date & Time             | `ses_wknd_r`         | Proportion of sessions on weekends                                                                     |
| Average Session Length                  | Other                   | `ses_len_avg`        | Average session duration (minutes)                                                                     |
| Interaction Time Gap                    | Other                   | `time_to_int`        | Average time between interactions (minutes)                                                            |
| Transaction Time Gap                    | Other                   | `time_to_tran`       | Average time between purchases (days)                                                                  |
| Inactivity Period                       | Engagement              | `inactive_days`      | Days since the user's last session relative to the reference date                                      |
| Peak Activity Hour                      | Engagement              | `peak_activity_hr`   | Hour of day (0-23) with the highest number of user interactions                                        |
| Peak Activity Day                       | Engagement              | `peak_activity_day`  | Day of the week (0-6, where 0=Monday) with the highest number of user interactions                     |
| Off-Hours Activity Rate                 | Engagement              | `off_hours_rate`     | Proportion of interactions occurring between 12 a.m. and 6 a.m.                                        |
| Session Length Standard Deviation       | Session Patterns       | `ses_len_sd`         | Standard deviation of session durations                                                                |
| Session Length Coefficient of Variation | Session Patterns       | `ses_len_cv`         | Ratio of std dev to mean session duration                                                              |
| Long Session Ratio                      | Session Patterns       | `long_ses_ratio`     | Proportion of sessions lasting more than 30 minutes                                                   |
| Short Session Ratio                     | Session Patterns       | `short_ses_ratio`    | Proportion of sessions lasting less than 5 minutes                                                    |
| Session Gaps Standard Deviation         | Session Patterns       | `ses_gap_sd`         | Standard deviation of time gaps between sessions (days)                                                |
| Interaction Recency                     | Interaction Behavior   | `int_rec`            | Days between the last interaction and the reference date                                               |
| Interaction Recency SD                  | Interaction Behavior   | `int_rec_sd`         | Standard deviation of time gaps between interactions (minutes)                                         |
| Average View-to-Cart Time               | Interaction Behavior   | `view_to_cart_avg`   | Average time taken to move from view to cart (minutes)                                                 |
| Average Cart-to-Purchase Time           | Interaction Behavior   | `cart_to_purchase_avg`| Average time taken to move from cart to purchase (minutes)                                             |
| Interaction Skewness                    | Interaction Behavior   | `int_skew`           | Skewness of interaction counts per session (measure of bias towards high/low activity)               |
| High Spending Spike Flag                | Revenue Patterns       | `high_spike_flag`    | 1 if there is a session with spending >2x average spending, else 0                                     |
| Revenue per Interaction                 | Revenue Patterns       | `rev_per_int`        | Total revenue divided by total number of interactions                                                  |
| Purchase Consistency                    | Revenue Patterns       | `purchase_consistency`| Standard deviation of spending per transaction                                                        |
| Popular Category Consistency            | Category & Item        | `pop_cat_consistency`| Fraction of sessions involving the most frequently interacted category                                 |
| Cross-Category Interaction Ratio        | Category & Item        | `cross_cat_ratio`    | Ratio of sessions with interactions in more than one category                                          |
| Churn Score                             | Other                   | `churn_score`        | Weighted score combining recency, frequency, monetary, and other behavioral metrics                   |
| Risk Category                           | Other                   | `risk_category`      | Categorization of user risk level (e.g., low, medium, high)                                           |
| Likely to Churn Flag                    | Other                   | `is_likely_churn`    | 1 if user is predicted to churn, else 0                                                                |
| Risk Velocity                           | Other                   | `risk_velocity`      | Rate at which the user’s risk of churn is increasing over time                                         |
| Primary Risk Drivers                    | Other                   | `primary_risk_drivers`| Main factors influencing the user's risk of churn                                                     |
| Estimated Days to Churn                 | Other                   | `estimated_days_to_churn`| Estimated number of days until the user is likely to churn                                             |
