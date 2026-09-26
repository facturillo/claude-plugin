# facturillo

Ask your facturillo receipts anything from Claude. facturillo keeps Panamanian receipts (facturas) organized automatically: scan the DGI QR code in the app and every line item, vendor and total is captured. This plugin connects Claude to your facturillo account, read-only, and teaches it how to answer questions about your real spending.

## Use it

Install the plugin, then connect the facturillo connector from the plugin's Connectors tab: a facturillo screen opens and you approve the connection in the facturillo app on your phone. Then ask in Spanish or English:

- "How much did I spend on groceries last month?"
- "Where did I buy milk, and what did it cost?"
- "Which store do I visit most?"
- "Show me my most recent receipt with every line item."
- "Which of my receipts has an attached document? Show it to me."

The `ask-your-receipts` skill tells Claude which facturillo tool answers which question (server-side summaries for totals, vendor profiles for "which store", product search in Spanish and English, receipt details and 15-minute document links) and how to handle family or business contexts.

## What it needs

A facturillo account (facturillo.com). The data features need an active facturillo plan; a free account can only verify the connection.

## Data

The plugin sends nothing on its own. Every question Claude answers with your data goes through the facturillo connector at `mcp.facturillo.com`, which reads your receipt data for that question only and never writes to your account. The connector is operated by facturillo Inc. under the facturillo privacy policy at https://facturillo.com/privacy (section "AI Assistant Connections"). Support: info@facturillo.com. Documentation: https://facturillo.com/ai.
