## Quick Overview

This workflow fetches live gold (XAU) and silver (XAG) prices from GoldAPI.io, calculates the gold-to-silver ratio, evaluates it against configurable buy/hold thresholds, and sends a formatted investment opportunity report via Gmail.

## How it works

1. Starts manually and loads configuration values such as the GoldAPI API key, currency, recipient email address, and ratio thresholds.
2. Retrieves the latest gold and silver prices from GoldAPI.io and extracts the required price values.
3. Combines both price feeds and calculates the current gold-to-silver ratio.
4. Compares the calculated ratio against predefined thresholds to determine whether to **Buy Silver**, **Buy Gold**, or **Hold**.
5. Generates a timestamped report containing the latest prices, ratio, trading signal, and a brief market interpretation.
6. Sends the complete investment opportunity report to the configured recipient using Gmail.

## Setup

1. Create a GoldAPI.io account, obtain your API key, and add it to the workflow configuration.
2. Connect your Gmail OAuth2 credentials in n8n.
3. Configure the recipient email address, preferred currency (such as USD or INR), and the buy/sell ratio thresholds.
4. Replace the Manual Trigger with a Schedule Trigger if you want the workflow to run automatically.

## Requirements

- [**n8n account** (Self-hosted or Cloud)](https://n8n.partnerlinks.io/om1efg2qgvwi)
- GoldAPI.io account and API key
- Gmail OAuth2 credentials
- Internet access to GoldAPI.io

## Customization

- **Threshold Values:** Adjust the buy-gold and buy-silver ratio thresholds based on your investment strategy.
- **Currency:** Change the currency code to retrieve prices in your preferred currency.
- **Email Template:** Customize the email subject, formatting, and investment insights.
- **Trigger Type:** Replace the manual trigger with a scheduled trigger for automated monitoring.

## Additional Info

### Who's It For

- Precious metals investors
- Financial advisors
- Portfolio managers
- Commodity traders
- Personal finance enthusiasts

### Add-ons & Enhancements

- Run automatically with a Schedule Trigger
- Store historical prices in Google Sheets
- Send Slack or Microsoft Teams notifications
- Add Telegram or SMS alerts
- Build historical trend dashboards
- Track multiple precious metals

### Use Case Examples

- Monitor gold-to-silver investment opportunities
- Receive automated precious metals alerts
- Track portfolio diversification signals
- Build long-term ratio history for market analysis
- Learn commodity market automation using n8n

### Troubleshooting Guide

| Issue | Possible Cause | Solution |
|--------|----------------|----------|
| No price data returned | Invalid or missing GoldAPI API key | Verify the API key and account status |
| Email not sent | Gmail credentials are missing or expired | Reconnect Gmail OAuth2 credentials |
| Ratio calculation is incorrect | Price fields are mapped incorrectly | Verify the field mappings from the API response |
| Workflow stops unexpectedly | Incorrect node configuration | Review node connections and workflow execution |
| Incorrect trading signals | Threshold values are not configured properly | Update the buy and hold threshold values |

## Need Help?

If you need help customizing this workflow, integrating it with your investment tracking systems, or extending it with AI-powered market insights, historical analytics, and multi-channel notifications, our **WeblineIndia** team is ready to assist. Explore our **[Process Automation Solutions](https://www.weblineindia.com/process-automation-solutions.html)** or connect with our **[n8n workflow development experts](https://www.weblineindia.com/n8n-automation/)** to build, customize, and scale your business automation with confidence.
