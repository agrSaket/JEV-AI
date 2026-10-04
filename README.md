# Customer Support Ticket Analyzer
> AI-powered customer support ticket classification and prioritization using the **TypeSafe SDK** and **JEV-AI model**.

## Overview
The **Customer Support Ticket Analyzer** analyzes customer support messages to identify the type of issue and measure customer frustration.

## Features
- **Frustration Detection:** Rates customer frustration from **1 (Calm) to 5 (Extremely Hostile/Urgent)**.
- **Natural Language Understanding:** Processes unstructured customer support messages.
- **Confidence-Based Analysis:** Returns classifications based on configured confidence thresholds.

## How It Works
```text
Customer Support Ticket
          │
          ▼
    TypeSafe SDK
          │
          ▼
      JEV-AI Model
          │
     ┌────┴────┐
     ▼         ▼
  Category   Frustration
     │         │
     └────┬────┘
          ▼
    Analysis Result
```
## Getting Started
### Requirements
- Python 3.x
- Google Colab
- TypeSafe API Key

### Run in Google Colab
1. Open `customer_support_ticket_analyzer.ipynb` in Google Colab.
2. Install the TypeSafe SDK:
```python
!pip install typesafe_sdk
```
3. Configure your TypeSafe API key:
```python
import os
os.environ["TYPESAFE_API_KEY"] = "your-api-key"
```
4. Run the notebook cells sequentially.
5. Enter customer support messages and review the generated analysis.

## Frustration Scale
The customer's frustration level is evaluated on a scale from **1 to 5**:
| Score | Level |
|------:|-------|
| **1** | Calm |
| **2** | Slightly Frustrated |
| **3** | Moderately Frustrated |
| **4** | Highly Frustrated |
| **5** | Extremely Hostile / Urgent |
   
## Supported Categories
| Category | Description |
|----------|-------------|
| **Software Bugs** | Application errors, crashes, or unexpected behavior |
| **Billing & Invoices** | Payment, invoice, refund, or billing-related issues |
| **Account Access** | Login, authentication, or password-related issues |
| **Feature Requests** | Requests for new features or product improvements |

## Technologies
- **Python**
- **Google Colab**
- **TypeSafe SDK**
- **JEV-AI Model**

## Project Structure
```text
customer-support-ticket-analyzer/
│
├── README.md
└── customer_support_ticket_analyzer.ipynb
```
## Future Improvements
- Add more ticket categories
- Support batch ticket analysis
- Integrate with customer support platforms
- Generate AI-powered response suggestions

⭐ If you find this project useful, consider giving it a star!
