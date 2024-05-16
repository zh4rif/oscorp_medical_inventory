Functional Requirements

1.User Authentication
Description:This functionality allows users to securely log in to the system using their staff ID and password. It ensures that only authorized personnel have access to the system.
Implementation Details:
Login Form:A login interface where users enter their staff ID and password.
Authentication:Verify credentials against a database.
Session Management:Create and manage user sessions using tokens to keep users logged in securely.
Security:Implement measures such as password hashing, account lockout after multiple failed attempts, and secure communication (HTTPS).

2. Manage Medicine Quantity
Description:This functionality allows users to add to or subtract from the inventory of medicines. This ensures accurate tracking of medicine stock levels.
Implementation Details:
Inventory Update Interface:Forms or buttons to increase or decrease the quantity of each medicine.
Database Operations:myPHPadmin operations to update inventory records.
Validation:Ensure quantities do not go negative and updates are logged for auditing purposes.


3.Medical Description Management
Description:Users can add and view detailed descriptions of medicines. This helps in providing comprehensive information about each medicine in the inventory.
Implementation Details:
Description Form:A form to enter and update the description of medicines.
Display Information:A detailed view to display medicine information including description, usage, dosage, and side effects.
Database Storage:Store and retrieve description data from the database.

4. Expiry Date Notifications
Description: This functionality alerts users when a medicine is about to expire or has expired. This ensures that expired medicines are not dispensed.
Implementation Details:
Expiry Date Tracking:Store expiry dates for each medicine batch.
Notification System:Periodic checks to identify medicines nearing expiry.
Alerts:Send notifications via email, SMS, or in-app alerts to users about upcoming or past expiry dates.

5. Medicine Search
Description:Users can search for medicines by name. This facilitates quick access to medicine information and inventory status.
Implementation Details:
Search Interface:A search bar where users can type in the medicine name.
Search Algorithm:Implement a search algorithm to match medicine names and provide suggestions as users type.
Results Display: Show a list of medicines that match the search query along with relevant details.

6. Low Stock Notifications
Description:This functionality alerts users when the stock of a medicine falls below a predefined threshold. This ensures timely reordering of medicines to avoid stockouts.
Implementation Details:
Stock Monitoring: Periodic checks to compare current stock levels with thresholds.
Alerts:Send notifications via email, SMS, or in-app alerts when stock falls below the threshold.

7.Purchase Order Generation
Description:Users can generate purchase orders for restocking inventory. This streamlines the process of ordering new stock from suppliers.
Implementation Details:
Order Form:A form to create new purchase orders, including medicine details, quantities, and supplier information.
Auto-Fill Features:Suggest medicines that are low on stock for quick order creation.
Order Management:Track the status of purchase orders such as pending, approved, received and generate order documents such as PDF.

8. Supplier Integration
Description:This allows real-time integration with supplier systems for inventory updates and ordering. This ensures seamless restocking and up-to-date inventory data.
Implementation Details:
API Integration: Connect with supplier systems using APIs to place orders and receive updates.
Real-Time Data:Use webhooks or similar technology to receive instant updates from suppliers about order status and inventory changes.
Order Synchronization: Ensure that orders placed through the system are reflected in both the local inventory and the supplier’s system.

9.Barcode Scanning
Description:Users can use barcode scanning to upload inventory stock data. This increases the efficiency and accuracy of inventory management.
Implementation Details:

Non-Functional Requirements

1. Compatibility
Description:The software must be compatible with and installable on both Android and iOS devices, ensuring that it can be accessed and used by a wide range of users across different mobile platforms.
Implementation Details:
Cross-Platform Development:Utilize frameworks like React Native or Flutter to develop a single codebase that works on both Android and iOS.
Testing:Conduct thorough testing on a variety of Android and iOS devices to ensure compatibility and performance.
App Store Compliance:Ensure the software meets the guidelines and requirements of both the Google Play Store and Apple App Store for distribution.

2. Load Handling
Description:The software must be capable of handling up to 100 concurrent users without performance degradation, ensuring smooth operation during peak usage times.
Implementation Details:
Scalability:Design the system architecture to be scalable, possibly using cloud services like AWS, Azure, or Google Cloud that can dynamically allocate resources based on demand.
Performance Testing:Use tools like JMeter or LoadRunner to simulate concurrent users and test the system's performance under load.
Optimized Code:Write efficient code and use performance optimization techniques such as caching, database indexing, and query optimization to ensure the system runs smoothly under load.

3. Security
Description:The software must be resilient against malware and virus attacks, protecting user data and maintaining the integrity of the system.
Implementation Details:
Secure Coding Practices: Follow secure coding practices to prevent common vulnerabilities such as SQL injection, cross-site scripting (XSS), and cross-site request forgery (CSRF).
Regular Security Audits: Perform regular security audits and penetration testing to identify and address potential vulnerabilities.
Antivirus Integration: Integrate antivirus and malware detection tools to scan and protect the system from malicious software.

Barcode Scanner Integration:Support for barcode scanners (handheld devices or mobile apps).
Data Parsing:Read and interpret barcode data to update inventory records.
Inventory Update:Automatically adjust inventory levels based on scanned data, including adding new stock and verifying existing quantities.
