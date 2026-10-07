- Application: practicesoftwaretesting.com v5.0
- Version: 1.0
- Date: 10/7/2026
- Author: Mohamed
# 1. Introduction & Objectives
The purpose of this document is to define the testing approach of the online tool shop *PracticeSoftwareTesting.com*. The main Objectives:
- Verify the store's main functionalities (search & filter products, manage carts, order & checkout, user login) work as expected.
- Write test automation scripts to facilitate regression tests for continues deployments.

# 2. Scope
## 2.1 In Scope:
- Search & filter products
- Products pagination
- Cart
- Order
- User profile (login & logout, saved address)
## 2.2 Out of Scope 
- Admin capabilities
- Mobile app
- Security / Penetration testing and Database direct inspection
- Performance and load tests

# 3. Test Strategy
- Test Level: System
- Test Type: Functional UI, Black-box
- Test Approach:
	- - Manual testing for exploratory and usability
	- Automation testing for regression using Playwright
# 4. Test Environment
## 4.1 Host URL
- https://www.practicesoftwaretesting.com
## 4.2 Devices

| Device                       | OS         | Browsers          |
| ---------------------------- | ---------- | ----------------- |
| Lenovo Laptop IDEAPAD Slim 3 | Windows 11 | Chromium, Firefox |
## 4.3 Tools

| Tool       | Purpose                                                  |
| ---------- | -------------------------------------------------------- |
| Obsiden    | documenting test cases, bug and test reports             |
| Playwright | automating test scripts                                  |
| DevTools   | inspect UI elements for selectors, read network activity |
## 4.4 Test Data
### Default accounts

| First name | Last name | Role | E-mail                                | Password  |
| ---------- | --------- | ---- | ------------------------------------- | --------- |
| Jane       | Doe       | user | customer@practicesoftwaretesting.com  | welcome01 |
| Jack       | Howe      | user | customer2@practicesoftwaretesting.com | welcome01 |
| Bob        | Smith     | user | customer3@practicesoftwaretesting.com | pass123   |
### Addresses
- Use fictional addresses from famous TV shows like Breaking Bad (308 Negra Arroyo Lane, Albuquerque, NM)
# 5. Test Deliverables
- Test cases
- Test report
- Bug reports
- Test scripts
# 6 Roles & Responsibilities

| Personnel     | Role        | Contacts                     | Responsibilities             |
| ------------- | ----------- | ---------------------------- | ---------------------------- |
| Mohamed       | QA Engineer | mohamedgisimelsied@gmail.com | write and execute test cases |
| Roy de Kleijn | Developer   | testsmith.io                 | Fix reported defects         |
# 7. Entry & Exit Criteria
## 7.1 Entry Criteria
- Hosted staging URL responds with HTTP 200.
- 5-minute Smoke Checklist passes (Login, Search, Add to Cart).
- Test cases are written and finalized.
## 7.2 Exit Criteria
- 100% of P0/P1 test cases executed.
- 0 open P0 (Blocker) bugs.
- Minimum 90% overall test pass rate.
- Final Test Summary Report published with test execution logs and open defect matrix.
# 8. Risks & Mitigation

| Risk                         | Mitigation             |
| ---------------------------- | ---------------------- |
| Test environment instability | use local docker image |
# 9. Test Schedule

| Activity             | Duration |
| -------------------- | -------- |
| Test planning        | 1.5 day  |
| Test case design     | 2 days   |
| Test execution       | 2 days   |
| Automation scripting | 3-4 fays |
| Test closure         | 1 day    |
- Start date: 10/7/2026