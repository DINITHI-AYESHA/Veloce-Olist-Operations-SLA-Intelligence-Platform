# Agile Project Backlog & User Stories

## Sprint 1: Executive Marketplace & Commercial Performance
### US-01: Executive GMV & Sales Dynamics
- **Priority:** High
- **User Story:** As a Chief Commercial Officer (CCO), I want to monitor total GMV, order volume, and category revenue distribution across Brazilian states, so that I can evaluate top-line marketplace growth and regional sales concentration.
- **Acceptance Criteria:**
  - Given customer orders marked as `delivered`,
  - When filtering by a selected purchase date range,
  - Then the KPI ribbon displays total GMV (excluding cancelled/unavailable orders), total distinct orders, average order value (AOV), and a breakdown of the top 10 product categories.

---

## Sprint 2: Logistics & Carrier SLA Performance
### US-02: Delivery Lead Time & SLA Breach Analysis
- **Priority:** Critical
- **User Story:** As a Head of Logistics & Supply Chain, I want to compare actual delivery transit days against estimated carrier SLA dates across destination states, so that I can identify regional carrier bottlenecks and minimize late-delivery penalties.
- **Acceptance Criteria:**
  - Given fulfilled orders with valid delivery and estimated delivery timestamps,
  - When calculating SLA variance (`order_delivered_customer_date` vs. `order_estimated_delivery_date`),
  - Then orders delivered past the estimated date flag as a breach, calculating an accurate SLA Breach Rate (%) and average delay duration in days per customer state.

---

## Sprint 3: Fulfillment Risk & Operations Bottlenecks
### US-03: Order Defect & Seller Shipping Lag
- **Priority:** Medium
- **User Story:** As an Operations Director, I want to measure the duration between order approval and carrier dispatch alongside cancellation volume, so that I can detect merchant dispatch delays before parcels reach the carrier network.
- **Acceptance Criteria:**
  - Given order lifecycle timestamps,
  - When measuring the delta between `order_approved_at` and `order_delivered_carrier_date`,
  - Then highlight seller dispatch lag outliers (>48 hours) and display cancellation rate trends over time.