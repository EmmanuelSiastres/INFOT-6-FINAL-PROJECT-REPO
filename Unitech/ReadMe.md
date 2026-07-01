**Integrated Performance Management System (IPMS) of University of Antique**

**Project Description**  
The Integrated Performance Management System (IPMS) is a web-based platform designed for the University of Antique to automate and digitize the Individual Performance Commitment and Review (IPCR) and Office Performance Commitment and Review (IPCR) and Office Performance Commitment and Review (OPCR) processes. It replaces manual, paper-based workflows with a centralized system that enables secure objective setting, real-time progress tracking, automated evaluation workflows, and advanced analytics for data-driven decision-making. The system supports role-based access for faculty, staff, and administrators to ensure transparency, accountability, and efficiency in performance management. 

**Team Info**

Name: Darry Alterado  
Role: Team Leader

Name: Therese Anne Baladiang  
Role: Data Analyst / Documentation

Name: Mary Trishia Tamaño  
Role: Developer

**API Endpoints**

Method: POST  
Endpoint: /api/auth/register  
Description: Register a new user (Admin only)  
Auth Required: No

Method: POST  
Endpoint: /api/auth/login  
Description: Login and receive JWT token  
Auth Required: No

Method: POST  
Endpoint: /api/auth/logout  
Description: Invalidate current session/token  
Auth Required: Yes

Method: GET  
Endpoint: /api/users/me  
Description: Get current user profile and role  
Auth Required: Yes

Method: POST  
Endpoint: /api/objectives  
Description: Create a new performance objectives (IPCR/OPCR)  
Auth Required: Yes  
Method: PUT  
Endpoint: /api/objectives/{id}  
Description: Update existing objectives  
Auth Required: Yes

Method: GET  
Endpoint: /api/objectives  
Description: List objectives (filtered by role)  
Auth Required: Yes

Method: POST  
Endpoint: /api/evaluations  
Description: Submit performance evaluation/rating  
Auth Required: Yes

Method: PUT  
Endpoint: /api/evaluations/{id}  
Description: Approved or reject an evaluation   
Auth Required: Yes (Admin/ Department Head)

Method: GET  
Endpoint: /api/analytics/trends  
Description: Retrieve historical performance trends  
Auth Required: Yes (Admin)

Method: Get  
Endpoint: /api/audit-logs  
Description: View system activity logs  
Auth Required: Yes (Admin)

Method: POST  
Endpoint: /api/notifications/send  
Description: Trigger manual notification  
Auth Required: Yes (Admin)

**Environment Variables**

Variable Name: APP\_ENV  
Purpose: Application environment (local/production)  
Value: local

Variable Name: APP\_URL  
Purpose: Base URL for the application  
Value: [http://127.0.0.1:8000](http://127.0.0.1:8000)

Variable Name: DB\_CONNECTION  
Purpose: Database driver  
Value: SQLite  
Variable Name: DB\_PORT  
Purpose: Database port  
Value: 8000

**AI DIsclosure**

In compliance with academic integrity policies, the following AI-assisted tools were used during the development of this project:

* Code Debugging & Optimization: GitHub Copilot was used to suggest syntax corrections and optimized SQL queries within the Laravel backend.  
* Documentation: AI tools assisted in drafting the initial structure of the API documentation and generating unit test cases. 

**Attribution**

This project utilizes the following open-source libraries and frameworks:

Library / Framework: Laravel  
Version: 5.25.1  
Purpose: Backend Framework for API and logic.

Library / Framework: SQLite  
Version: 3.x  
Purpose: Lightweight, serverless relational database for local storage.

Library / Framework: Tailwind CSS  
Version: 3.x  
Purpose: Utility-first CSS framework for styling.

Library / Framework: Bcrypt  
Version: latest  
Purpose: Password hashing and security. 

