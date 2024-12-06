# Evershop Ecommerce Testing

**Role:** Manual Tester  
**Tools:** Postman, Google Sheets

## Project Overview
This project involves testing the search functionality, cart operations, and final checkout process of the **Evershop Demo Ecommerce** site. The testing was conducted through both **UI** and **API** methods to ensure a smooth user experience and proper performance. Comprehensive test cases were written and executed, and defects were tracked manually.

## Testing Scope

### UI Testing
- Tested the entire process from search to adding items to the cart and completing checkout.
- Identified several UI issues, such as product color auto-changing, cart behavior on screen resize, input validation anomalies, and payment method issues.

### API Testing (Postman)
- API endpoints from search to checkout were tested for accuracy and performance.
- Documented the behavior of various API methods, including `GET`, `POST`, `PATCH`, and `DELETE`.
- Found minor issues like session-dependent behavior and mismatches in the final checkout subtotal.

## Key Findings

### UI Issues:
1. **Product Color Auto-Change:**  
   Size selection defaults color to pink.
2. **Cart Behavior on Resize:**  
   Items reappear visually when resizing the screen.
3. **Input Field Validation:**  
   No validation in fields; non-shippable countries are selectable.
4. **Payment & Checkout Anomalies:**  
   Visa card input fails, and the "Thank You" screen shows an incorrect item subtotal.

### API Findings:
- **Search API:** Works correctly, matches UI results.
- **Cart API:** Functions properly but fails when tested without an active session.
- **Delete Product API:** Fails with a 500 error in Postman due to potential session or input validation issues.
- **Final Checkout API:** Works, but UI mismatches in the displayed subtotal.

## Conclusion
The project revealed several UI issues and some session-dependent behaviors in the APIs. While the APIs generally performed well, further development is required for smoother integration with the UI.
