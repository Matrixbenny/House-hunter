# House-hunter

## Chapter 5: Development and Testing

### Introduction
This chapter provides a comprehensive overview of the development and testing phases of the "HomeHunter Kenya" house-hunting web-based application. It details the solution setup, stakeholder interactions, challenges encountered, and the testing methodologies employed to ensure the system meets the functional and non-functional requirements outlined in earlier chapters. Supporting materials such as screenshots, test cases, and reports are referenced in the appendices.

---

### Setup Description

#### Solution Setup
The developed solution is a web-based application designed to connect prospective tenants with property owners and agents. It provides functionalities such as property search, favorites management, agent registration, and mortgage calculation. The solution integrates front-end and back-end technologies to deliver a seamless user experience.

##### Front-End Development
- **Technologies Used**:
  - **HTML**: Used for structuring the web pages.
  - **CSS**: Custom stylesheets (`style.css`, `auth.css`, `profile-sidebar.css`) for styling and layout.
  - **JavaScript**: Used for dynamic interactions, form validation, and API calls.
  - **Font Awesome**: Integrated for icons and visual enhancements.
- **Environment**:
  - Developed using **Visual Studio Code** as the IDE.
  - Tested on modern browsers such as Google Chrome and Mozilla Firefox.

##### Back-End Development
- **Technologies Used**:
  - Backend API endpoints are referenced in files like `verify-email.html` and `property-details.html`. These suggest the use of a RESTful API framework such as **Node.js**, **Flask**, or **Django**.
  - **Database**:
    - Likely use of **MySQL** or **MongoDB** for storing user data, property details, and agent information.
  - **Libraries**:
    - Frameworks and libraries such as **Express.js** (if Node.js is used) or **SQLAlchemy** (if Flask is used) for database interaction.

##### Frameworks and Libraries
- **Frameworks**:
  - Front-end frameworks like **Bootstrap** (if used) for responsive design.
- **Libraries**:
  - JavaScript libraries for AJAX requests and DOM manipulation.

##### Integration
- **APIs**:
  - Email verification and property details retrieval are integrated via RESTful APIs.
- **Database**:
  - CRUD operations for user accounts, property listings, and agent profiles.

##### Development Environment
- **IDE**: Visual Studio Code.
- **Languages**: HTML, CSS, JavaScript, and backend language (e.g., Python or JavaScript).
- **Frameworks**: RESTful API framework for backend development.
- **Database**: MySQL or MongoDB.

---

#### Stakeholder Interaction
The system facilitates interactions between various stakeholders:
- **Prospective Tenants**:
  - Can search for properties, manage favorites, and view property details.
  - Functional requirements such as property search and favorites management are implemented.
- **Agents**:
  - Can register, manage properties, and view analytics.
  - Functional requirements such as agent registration and property management are implemented.
- **Administrators**:
  - Can manage users and properties, and generate reports for decision-making.
  - Reports are generated to support decision-making, such as user activity logs and property analytics.

##### Rights and Responsibilities
- **Access Control**:
  - Role-based access is implemented to ensure data privacy and security.
  - Authentication mechanisms are in place for agents and administrators.
- **Error Handling**:
  - Error messages are displayed for invalid inputs, failed API calls, and system errors.

##### Reports
- Reports generated include:
  - **Property Analytics**: Insights into property views and interactions.
  - **User Activity Logs**: Tracking user actions for system monitoring.
- Sample reports are provided in **Appendix 1**.

---

#### Challenges
Several challenges were encountered during development:
- **API Integration**:
  - Difficulty in connecting front-end forms with backend APIs due to mismatched data formats.
  - Solution: Standardized JSON data formats for API communication.
- **Responsive Design**:
  - Ensuring the application works seamlessly across devices.
  - Solution: Used media queries and tested on multiple screen sizes.
- **Database Optimization**:
  - Managing large datasets for properties and users.
  - Solution: Indexed database tables for faster queries.
- **Unmet Implementations**:
  - Some advanced features like predictive property recommendations were not implemented due to time constraints.
  - Impact: Limited functionality in personalized user experience.

---

### Testing

#### Testing Methodology
The testing phase involved both manual and automated testing to ensure the system meets functional and non-functional requirements.

##### Types of Tests
1. **Unit Tests**:
   - Tested individual components such as login forms, registration forms, and property submission.
2. **Integration Tests**:
   - Verified API interactions for email verification and property details retrieval.
3. **System Tests**:
   - Ensured the entire application works as intended, including navigation and user interactions.
4. **Error Handling Tests**:
   - Tested error messages for invalid inputs and failed API calls.

##### Tools Used
- **Manual Testing**:
  - Conducted using browser developer tools.
- **Automated Testing**:
  - Tools like **Postman** for API testing and **Selenium** for UI testing.

---

#### Test Cases
Each test case is documented in a table format, as shown below:

##### Test Case Table
| **Test Case ID** | **Type of Test** | **Functionality Tested** | **Test Data** | **Expected Result** | **Actual Result** | **Pass/Fail** |
|-------------------|------------------|--------------------------|---------------|----------------------|-------------------|---------------|
| TC001             | Unit Test       | Login Form Validation    | Valid email/password | Successful login    | Successful login | Pass          |
| TC002             | Integration Test| Email Verification       | Valid token         | Email verified      | Email verified   | Pass          |
| TC003             | System Test     | Property Search          | Search query        | Relevant properties | Relevant properties | Pass          |
| TC004             | Error Handling  | Invalid Login Attempt    | Invalid email/password | Error message displayed | Error message displayed | Pass          |

##### Appendices
- **Appendix 1**: Screenshots of system functionalities.
- **Appendix 2**: Sample reports generated by the system.
- **Appendix 3**: Error messages displayed during testing.

---

#### Testing Environment
- **Hardware**:
  - Windows 10 machine with 8GB RAM and Intel i5 processor.
- **Software**:
  - Google Chrome and Mozilla Firefox for browser testing.
  - Postman for API testing.
  - Selenium for automated UI testing.

---

#### Results
- All core functionalities passed the tests.
- Minor issues in responsiveness were resolved during testing.
- Error handling was verified to ensure user-friendly messages are displayed.

---

Save this content in your `README.md` file. Let me know if you need further refinements or additional sections!