# Veridi Logistics Last-Mile Delivery Audit

## A. Executive Summary

## Executive Summary

Veridi Logistics needed to assess whether negative customer reviews were linked to late deliveries and inaccurate delivery promises. Using the Olist Brazilian E-Commerce dataset, the project merged order, customer, review, and location data, cleaned missing and duplicate records, and classified deliveries as On Time, Late, or Super Late. The analysis found that most orders arrived on time, while  8.11% were late. Late deliveries were concentrated in states such as **AL** and **MA**, showing that the issue was regional rather than countrywide. Super late deliveries received the lowest review scores, confirming that delivery delays reduced customer satisfaction.

## B. Project Links

- **Link to Notebook:** https://drive.google.com/file/d/1ffVcAG2o0_CD-Z_U__z7-wmGpKiBqBNK/view?usp=sharing
- **Link to Dashboard:** https://amalitech-logistics-hwwt9zpcppbw45ea3dbt7s.streamlit.app/
- **Link to Presentation:** https://drive.google.com/file/d/1aovfA1Ml5AoolwGj0Tf02YGotnIxq4eQ/view?usp=sharing

## C. Technical Explanation

### Data Cleaning

The orders, customers, and reviews datasets were merged into one master dataset using `order_id` and `customer_id`. Duplicate reviews were handled by keeping the latest review for each order to avoid one-to-many duplicate records. Delivery date columns were converted to datetime format, and orders with missing delivery dates were separated as not delivered. Missing review scores were excluded before customer satisfaction analysis, and missing product category values were excluded before analyzing late delivery by product category.

### Candidate's Choice

The candidate's choice feature was the monthly late delivery trend. This feature matters because it shows the months where delivery risk increases, especially March and November, helping the business plan logistics resources earlier.

