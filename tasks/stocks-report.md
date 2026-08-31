# 📊 Daily Market Performance Report

Every day at **6:00 PM IST (18:00 India Standard Time)**, provide a short performance report for the **stocks, mutual funds, ETFs, or other securities** listed below.

---

## 📌 Securities to Track

Replace the examples below with the securities you want to monitor:

1. **ICICI Prudential Nifty Midcap 150 Index Fund**
2. **Nippon India Index Fund - Nifty 50 Plan**

---

## 📈 Report Requirements

For **each security**, report only the following information:

### 1. Today's Performance

Show the percentage change for the current trading day, including the `+` or `-` sign.

Examples:

- `+0.371%`
- `-0.226%`

### 2. Today's NAV / Price

Show today's latest available **NAV or closing price**, depending on the type of security.

- Mutual Fund → NAV
- Stock → Closing Price
- ETF → Closing Market Price
- Other securities → Use the appropriate official price/value

### 3. Previous Trading Day's NAV / Price

Show the NAV or price from the **previous trading day**.

Do **not** use the previous calendar day if it was a weekend or market holiday.

### 4. Price Movement

Calculate the absolute price movement using:

**Price Movement = Today's NAV/Price − Previous Trading Day's NAV/Price**

Show the result with a `+` or `-` sign.

Examples:

- `+₹1.02`
- `-₹0.36`

---

## 📋 Output Format

Keep the report **very short** and use the following format:

### Daily Market Report — DD/MM/YYYY

| Security | Today's Performance | Today's NAV/Price | Previous NAV/Price | Price Movement |
|---|---:|---:|---:|---:|
| Security 1 | +0.371% | ₹XXX.XX | ₹XXX.XX | +₹1.02 |
| Security 2 | -0.226% | ₹XXX.XX | ₹XXX.XX | -₹0.36 |

---

## ⚙️ Rules

1. Use **official or highly reliable market/fund data sources** whenever possible.
2. Use the **latest available data for the current trading day**.
3. For mutual funds, use **NAV**, not the market price.
4. For stocks and ETFs, use the appropriate **official/latest closing price**.
5. Compare today's value with the **previous trading day's** value.
6. Do not compare against the previous calendar day when that day was a weekend or market holiday.
7. Calculate price movement directly from the two NAV/price values:

   `Today's NAV/Price − Previous Trading Day's NAV/Price`

8. Do **not** calculate the rupee movement by simply converting the percentage change.
9. Include the `+` or `-` sign for both percentage performance and price movement.
10. Preserve the actual precision of the reported NAV/price whenever possible.
11. If today's data is not yet available, clearly state:

    `Data not available yet`

    Do not estimate or use unofficial values.
12. Do not include lengthy explanations, market news, predictions, analysis, or investment advice.
13. Keep the report focused only on the requested numbers.
14. If the market/fund did not trade or publish a NAV on a particular day, use the most recent **previous trading day** as the comparison point.

---

## 🕕 Schedule

Generate this report automatically:

**Every day at 6:00 PM IST (18:00 India Standard Time).**

---
