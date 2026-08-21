# HRM & Payroll – Test Scenarios

## 1. Employee Management

| ID          | Test Scenario                                | Expected Result                                                 |
| ----------- | -------------------------------------------- | --------------------------------------------------------------- |
| HRM-EMP-001 | Create a new employee with valid information | Employee should be created successfully                         |
| HRM-EMP-002 | Create employee with mandatory fields empty  | System should display appropriate validation messages           |
| HRM-EMP-003 | Create employee with duplicate Employee ID   | System should prevent duplicate Employee ID                     |
| HRM-EMP-004 | Edit existing employee information           | Updated information should be saved correctly                   |
| HRM-EMP-005 | Search employee by Employee ID               | Correct employee should be displayed                            |
| HRM-EMP-006 | Search employee by name                      | Matching employees should be displayed                          |
| HRM-EMP-007 | Deactivate an employee                       | Employee should become inactive and follow system rules         |
| HRM-EMP-008 | Verify employee information after update     | Updated information should be reflected across relevant modules |

---

## 2. Attendance Management

| ID          | Test Scenario                                             | Expected Result                                                       |
| ----------- | --------------------------------------------------------- | --------------------------------------------------------------------- |
| HRM-ATT-001 | Import attendance data from biometric device              | Attendance records should be imported correctly                       |
| HRM-ATT-002 | Verify employee attendance for a specific date            | Correct attendance status should be displayed                         |
| HRM-ATT-003 | Verify Check-In and Check-Out time                        | Correct time should be displayed                                      |
| HRM-ATT-004 | Process attendance for an employee with missing Check-Out | System should handle missing attendance according to configured rules |
| HRM-ATT-005 | Verify late attendance                                    | Late status should be calculated correctly                            |
| HRM-ATT-006 | Verify attendance after manual adjustment                 | Adjusted attendance should be reflected correctly                     |
| HRM-ATT-007 | Approve attendance adjustment                             | Approved adjustment should update attendance accordingly              |
| HRM-ATT-008 | Verify duplicate attendance records                       | System should prevent or properly handle duplicate records            |
| HRM-ATT-009 | Verify attendance synchronization                         | Device attendance should be synchronized with HRM correctly           |

---

## 3. Leave Management

| ID          | Test Scenario                                 | Expected Result                                                 |
| ----------- | --------------------------------------------- | --------------------------------------------------------------- |
| HRM-LVE-001 | Apply for leave with valid information        | Leave application should be submitted successfully              |
| HRM-LVE-002 | Apply for leave without mandatory information | Validation message should be displayed                          |
| HRM-LVE-003 | Apply for leave exceeding available balance   | System should prevent or handle the request according to policy |
| HRM-LVE-004 | Approve leave application                     | Leave status should become approved                             |
| HRM-LVE-005 | Reject leave application                      | Leave status should become rejected                             |
| HRM-LVE-006 | Verify leave balance after approval           | Leave balance should be updated correctly                       |
| HRM-LVE-007 | Verify different leave types                  | Correct leave type should be applied                            |
| HRM-LVE-008 | Verify leave report                           | Report should show accurate leave information                   |

---

## 4. Overtime Management

| ID         | Test Scenario                                | Expected Result                                           |
| ---------- | -------------------------------------------- | --------------------------------------------------------- |
| HRM-OT-001 | Calculate overtime for eligible employee     | OT should be calculated according to configured rules     |
| HRM-OT-002 | Verify overtime based on attendance duration | Correct OT duration should be calculated                  |
| HRM-OT-003 | Verify OT rate calculation                   | OT amount should be calculated using the configured rate  |
| HRM-OT-004 | Verify employee without OT eligibility       | OT should not be generated where policy does not allow it |
| HRM-OT-005 | Verify maximum OT limit                      | System should enforce configured OT limits                |
| HRM-OT-006 | Verify OT amount in payroll                  | Approved OT should be reflected correctly in salary       |

---

## 5. Payroll & Salary

| ID          | Test Scenario                            | Expected Result                                                |
| ----------- | ---------------------------------------- | -------------------------------------------------------------- |
| HRM-PAY-001 | Generate monthly salary                  | Salary should be generated successfully                        |
| HRM-PAY-002 | Verify salary based on attendance        | Salary calculation should reflect attendance rules             |
| HRM-PAY-003 | Verify absent deduction                  | Correct absent deduction should be applied                     |
| HRM-PAY-004 | Verify late deduction                    | Late deduction should be calculated according to configuration |
| HRM-PAY-005 | Verify overtime payment                  | Approved OT amount should be included in salary                |
| HRM-PAY-006 | Verify increment in salary               | Incremented salary should be reflected correctly               |
| HRM-PAY-007 | Verify loan deduction                    | Applicable loan deduction should be included                   |
| HRM-PAY-008 | Verify PF calculation                    | PF amount should be calculated according to configured rules   |
| HRM-PAY-009 | Verify salary after payroll modification | Updated calculation should be reflected correctly              |
| HRM-PAY-010 | Verify final salary payable              | Net payable amount should be accurate                          |

---

## 6. Recruitment

| ID          | Test Scenario                       | Expected Result                                                        |
| ----------- | ----------------------------------- | ---------------------------------------------------------------------- |
| HRM-REC-001 | Create recruitment request          | Recruitment request should be created successfully                     |
| HRM-REC-002 | Add candidate information           | Candidate information should be saved correctly                        |
| HRM-REC-003 | Update candidate status             | Candidate status should be updated correctly                           |
| HRM-REC-004 | Move selected candidate to employee | Candidate information should be transferred correctly where applicable |

---

## 7. Employee Loan

| ID           | Test Scenario                       | Expected Result                               |
| ------------ | ----------------------------------- | --------------------------------------------- |
| HRM-LOAN-001 | Create employee loan request        | Loan request should be submitted successfully |
| HRM-LOAN-002 | Approve employee loan               | Loan should be approved successfully          |
| HRM-LOAN-003 | Verify monthly loan deduction       | Correct deduction should be generated         |
| HRM-LOAN-004 | Verify loan balance after deduction | Remaining balance should be updated correctly |

---

## 8. Increment & Promotion

| ID          | Test Scenario                   | Expected Result                                             |
| ----------- | ------------------------------- | ----------------------------------------------------------- |
| HRM-INC-001 | Apply salary increment          | Increment should be recorded successfully                   |
| HRM-INC-002 | Verify increment effective date | New salary should become effective from the configured date |
| HRM-INC-003 | Promote employee                | Promotion information should be updated correctly           |
| HRM-INC-004 | Verify promoted employee salary | Salary should reflect applicable promotion changes          |

---

## 9. Reports

| ID          | Test Scenario                                   | Expected Result                                                |
| ----------- | ----------------------------------------------- | -------------------------------------------------------------- |
| HRM-RPT-001 | Generate attendance report                      | Accurate attendance report should be generated                 |
| HRM-RPT-002 | Generate leave report                           | Accurate leave information should be displayed                 |
| HRM-RPT-003 | Generate salary report                          | Salary report should contain accurate payroll data             |
| HRM-RPT-004 | Export report                                   | Report should be exported successfully in the supported format |
| HRM-RPT-005 | Verify report data against database/application | Report data should match the source records                    |

---

## 10. Role & Permission Testing

| ID          | Test Scenario                                   | Expected Result                                              |
| ----------- | ----------------------------------------------- | ------------------------------------------------------------ |
| HRM-SEC-001 | Login with valid credentials                    | User should be logged in successfully                        |
| HRM-SEC-002 | Login with invalid credentials                  | Appropriate error message should be displayed                |
| HRM-SEC-003 | Access restricted module with unauthorized user | Access should be denied                                      |
| HRM-SEC-004 | Verify role-based permissions                   | User should only access permitted functions                  |
| HRM-SEC-005 | Verify approval permission                      | Only authorized users should be able to approve transactions |

---

## Testing Coverage

This test scenario collection covers major HRM business workflows:

**Employee → Attendance → Leave → OT → Payroll → Loan → Increment → Promotion → Reports → User Permissions**

These scenarios are designed based on practical ERP/HRM business processes and can be expanded into detailed test cases with test data, preconditions, execution steps, actual results, and defect references.
