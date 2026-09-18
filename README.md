# Marketplace Delivery SLA Analysis

A short exploratory analysis of e-commerce order delivery data, checking whether couriers are meeting their promised delivery timelines (SLA).

## What it does

- Loads raw order data (`task1_marketplace_delivery_sla_raw.csv`)
- Cleans and parses order/shipping/delivery dates
- Filters out test orders and computes actual delivery duration vs. the promised SLA (`promised_days`)
- Flags each order as **On Time** or **Late**
- Aggregates on-time delivery rate by courier
- Visualizes results with bar charts (on-time rate %, eligible vs. on-time order counts)

## Files

| File | Description |
|---|---|
| `marketplace_delivery_sla.ipynb` | Main analysis notebook (Colab-ready) |
| `task1_marketplace_delivery_sla_raw.csv` | Raw order data: order/customer IDs, dates, city, courier, payment/order status, promised SLA days, order value |

## Running it

Open `marketplace_delivery_sla.ipynb` in Jupyter or Google Colab (there's a badge at the top of the notebook) and run the cells in order. Requires `pandas`, `numpy`, `matplotlib`, and `seaborn`.

## Notes

- The raw CSV has total of 10 row and 13 column data and column (delivered_at) has one NaT value which does not needs to be handled as code itself handles the cleaning
