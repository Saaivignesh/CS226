
# Food Delivery Orders XML + DTD

## Decision

When and how should a customer’s food order be prepared and delivered on time?

## Signals (5–7)

-   Restaurant name — [Restaurant]
-   Order items and quantity — [Menu/Order]
-   Total price (with tax/fees) — [Payments]
-   Payment status (Paid/Unpaid) — [Payments]
-   Delivery method (Pickup or Delivery) — [Logistics]
-   Delivery address — [Location]
-   Estimated delivery time (in minutes) — [Logistics]

## Gaps

Live kitchen status updates (e.g., whether food is being prepared or delayed) are not included, which may affect accuracy of ETA.

## Risk

If the ETA or payment status is wrong or stale, orders may arrive late or unpaid, frustrating both the customer and the restaurant.

## Stewardship

Customer order data should only be shared between the customer, restaurant, and delivery staff. It should be securely stored and retained only for a short time (e.g., 90 days), then archived or deleted in compliance with data privacy rules.

## Data Domain

Primary — [Food Delivery Orders]  
Adjacent — [Payments], [Logistics/Location]

AI Use: Draft text and signals were brainstormed with the assistance of an AI tool (OpenAI ChatGPT).


