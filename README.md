# hackathon3-day5-
Testing Report
Project: Furniro E-Commerce Website
Day 5: Testing and Backend Refinement
Overview
This report outlines the testing results conducted on Day 5 of the project, focusing on backend optimization and overall performance improvements.

API Testing
Tool Used: Postman
Objective: Ensure proper functionality of all API endpoints.
Results:
Endpoint
Request Type
Response Time (ms)
Status Code
Remarks
/api/products
GET
200
200
Data fetched successfully.
/api/products/:id
GET
250
200
Product details loaded.
/api/cart/add
POST
300
201
Item added to cart successfully.
/api/checkout
POST
500
200
Checkout completed successfully.


Performance Testing
Tool Used: Lighthouse
Objective: Assess performance metrics and identify areas for optimization.
Results:
Metric
Score
Remarks
First Contentful Paint
1.6s
Acceptable performance for desktop.
Largest Contentful Paint
2.5s
Optimized after implementing lazy loading.
Speed Index
10.7s
Improvement needed for mobile devices.
Performance Score
65/100
Below optimal, caching strategies planned.


Security Testing
Tool Used: OWASP ZAP
Objective: Identify vulnerabilities and potential threats.
Results:
Test Type
Status
Remarks
Input Validation
Passed
All forms handle inputs securely.
Authentication Mechanisms
Passed
Secure login with hashed passwords verified.
API Security
Partial Pass
Some endpoints lack rate-limiting.
Cross-Site Scripting (XSS)
Passed
No vulnerabilities detected.


Image Optimization
Tool Used: TinyPNG
Objective: Reduce image sizes without quality loss.
Results:
Image Count
Original Size (MB)
Optimized Size (MB)
Reduction (%)
50
120
85
29%


Conclusions
API endpoints perform well under typical load but need improvements in handling high traffic.
Performance on mobile requires attention, focusing on speed index and resource caching.
Security testing revealed minor gaps, such as the need for rate-limiting on sensitive endpoints.

