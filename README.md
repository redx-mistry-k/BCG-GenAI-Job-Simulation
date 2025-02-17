# BCG-GenAI-Job-Simulation
Financial Chatbot Documentation
Version 1.0
Overview
This chatbot provides financial insights for Apple, Microsoft, and Tesla using historical data
(2022–2024). It analyzes metrics like revenue, net income, debt ratios, market share, and
growth trends. Built with Python and pandas, it uses keyword matching and year detection to
generate responses.
How It Works
1. Data Structure:
o Financial data stored in a pandas DataFrame with metrics across 3 years.
o Metrics include revenue, net income, cash flow, debt ratios, market share, and
growth percentages.
2. Query Processing:
o Converts queries to lowercase for case-insensitive matching.
o Uses regex to detect years (e.g., "2023") or defaults to the latest year (2024).
o Identifies companies (Apple/Microsoft/Tesla) from keywords.
3. Response Logic:
o Matches keywords (e.g., "revenue growth," "profit margin") to predefined
calculations.
o Handles comparative queries (e.g., "Compare Apple's debt ratios across
years").
o Formats large numbers as billions (e.g., "$383B") for readability.
Predefined Queries
The chatbot supports:
1. Single-Metric Analysis
• "What was [Company]'s revenue in [Year]?"
• "What is Tesla's 2023 net income?"
• "Show Microsoft's 2024 debt-to-asset ratio."
2. Growth Trends
• "How did Apple's revenue grow from 2022 to 2024?"
• "What was Tesla's net income growth in 2023?"
3. Comparisons
• "Compare Microsoft's profit margins over time."
• "What is Apple's market share trend?"
4. Financial Health
• "What was Tesla's cash flow in 2022?"
• "What is Microsoft's 2024 ROE?"
5. Market Analysis
• "What is Apple's market share in 2023?"
Limitations
1. Data Scope:
o Only supports Apple, Microsoft, Tesla (2022–2024 data).
o Cannot answer questions about other companies or years.
2. Query Flexibility:
o Requires specific keywords (e.g., "revenue," "debt ratio").
o Cannot handle complex calculations (e.g., custom financial ratios).
3. Comparative Analysis:
o Limited to single-company comparisons over time.
o No cross-company comparisons (e.g., "Compare Apple and Microsoft's
revenue").
4. Real-Time Data:
o Uses static historical data; no live market updates.
Example Usage
plaintext
Copy
User: "What was Microsoft's revenue growth between 2023 and 2024?"
Bot: "Microsoft's revenue grew by 15.7% from 2023 to 2024."
User: "Show Tesla's 2022 profit margin."
Bot: "Tesla's 2022 profit margin was 15.5%."
User: "What is Apple's cash flow in 2024?"
Bot: "Apple's 2024 operating cash flow was $118.3B."
Conclusion
This chatbot serves as a tool for quick financial analysis of major tech companies, ideal for
investors or students exploring historical financial trends. While limited in scope, it provides
accurate, formatted responses for common queries. Future improvements could include
expanding the dataset and adding natural language processing (NLP) for more flexible
interactions.
