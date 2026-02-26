**SDLC (Software Development Life Cycle)** is a structured process followed by the software industry to design, develop, and deliver high quality product to the customer.



**Phases:**

1. Requirement Analysis

2\. Design

3\. Development

4\. Testing

5\. Deployment

6\. Maintenance



Goal: Build the product.



**STLC (Software Testing Life Cycle)** is a structured process followed by the QA team to produce the product without bugs with high-quality.



**Phases:**

1. Requirement Analysis

2\. Test Planning

3\. Test Case Design

4\. Test Environment Setup

5\. Test Execution

6\. Test Closure



Goal: Ensure the quality of the product.



SDLC focuses on developing the software, whereas STLC focuses specifically on validating and verifying the software quality.



| **Verification        			| Validation**              		|

| **-------------------------------------	| ------------------------------------- |**

| Process-oriented    			| Product-oriented        		|

| No code execution   			| Requires code execution 		|

| Done before testing 			| Done after development  		|

| Static testing      			| Dynamic testing         		|

| Prevents defects    			| Detects defects         		|

| **Example Activities:**			| **Example Activities:			|**

| 1. Requirement review			| 1. Functional testing			|

| 2. Design review			| 2. Regression testing			|

| 3. Code review			| 3. System testing			|

| 4. Test case review			| 4. UAT 				|

| 5.Walkthroughs \& inspections		|(User Acceptance Testing)		|

| “Are we building the product right?” 	| Are we building the right product?”	|



Verification ensures we are building the product correctly according to specifications through reviews and static testing. Validation ensures we are building the right product by executing the application and performing dynamic testing.

Verification is about process compliance; Validation is about product correctness.



**Software testing** is the process of evaluating a software application to identify defects and ensure it meets the requirements and works as expected.



**Basic Types of Testing**



**Manual Testing** – Human testers execute test cases without automation tools.

**Automation Testing** – Test scripts are written using tools like Selenium, TestNG, JUnit, etc.



| **Feature          | Manual Testing                               | Automation Testing**                          |

| ---------------- | -------------------------------------------- | ------------------------------------------- |

| \*\*Definition\*\*   | Test cases are executed manually by a tester | Test cases are executed using tools/scripts |

| \*\*Speed\*\*        | Slower, takes more time                      | Faster, especially for repeated tests       |

| \*\*Accuracy\*\*     | Prone to human error                         | More accurate (if scripts are correct)      |

| \*\*Cost\*\*         | Lower initial cost                           | Higher initial cost (tools, scripts)        |

| \*\*Best For\*\*     | Exploratory, usability, ad-hoc testing       | Regression, load, repetitive test cases     |

| \*\*Tools Used\*\*   | None or basic tools (Excel, TestLink)        | Selenium, TestNG, JUnit, Cypress, etc.      |

| \*\*Skill Needed\*\* | Functional knowledge of app                  | Programming + testing knowledge             |



**Levels of Testing**



**Unit Testing** – Test individual functions or methods (by developers)

**Integration Testing** – Test how modules work together

**System Testing** – Test the complete application

**Acceptance Testing** – Test if the system meets business needs (e.g. UAT)



**Testing Types**



**Functional Testing** – Validates what the system does (e.g. login works)

**Non-functional Testing** – Validates how the system works (e.g. performance, security)

**Regression Testing** – Ensure old features still work after changes

**Smoke Testing** – Basic tests to ensure critical functionalities are working

**Sanity Testing** – Quick checks after minor changes



**| Smoke Testing            | Sanity Testing                |**

**| ------------------------ | ----------------------------- |**

| Broad testing            | Narrow testing                |

| Done on new build        | Done after bug fix            |

| Checks overall stability | Checks specific functionality |

**Smoke testin**g verifies basic build stability, while **sanity testing** validates specific functionality after minor changes.

In our project, we perform smoke testing after every deployment and sanity testing after critical bug fixes to ensure minimal regression impact.



**| Alpha                  | Beta                   |**

| ---------------------- | ---------------------- |

| Internal testing       | External testing       |

| Controlled environment | Real-world environment |

| Conducted by QA        | Conducted by end users |

**Alpha testing** is internal testing performed before releasing to users, whereas **beta testing** is done by real users in real environments.



**| Black Box         | White Box               |**

**| ----------------- | ----------------------- |**

| No code knowledge | Code knowledge required |

| Functional focus  | Structural focus        |

| QA role           | Developer role          |





**Common Testing Terms**



**Bug / Defect** – A flaw in the software

**Test Case** – A set of actions to verify a feature

**Test Plan** – A document outlining scope, approach, and resources

**Test Scenario** – A high-level description of what to test

**Test Data** – The input used during testing

E**xpected Result** – What the application should do



**Testing fundamentals**



**Static testing** is done without executing the application, mainly through reviews. **Dynamic testing** involves executing the application to validate functionality.



**| Static Testing       | Dynamic Testing                   |**

**| -------------------- | --------------------------------- |**

| No execution of code | Code execution required           |

| Done early           | Done after build                  |

| Prevents defects     | Detects defects                   |

| Cheaper              | More costly if defects found late |



**| Test Plan           | Test Strategy             |**

**| ------------------- | ------------------------- |**

| Project-specific    | Organization-level        |

| Detailed document   | High-level document       |

| Created per project | Created once              |

| Contains timeline   | Contains testing approach |

Test strategy defines the overall testing approach at organizational level, whereas test plan is a project-specific document describing scope, timeline, and execution details.



**| Bug Leakage            					| Defect Density           						|**

**| ------------------------------------------------------------- | --------------------------------------------------------------------- |**

| Found in production    					| Found during testing   						|

| Measures QA efficiency 					| Measures product quality 						|

| **Formula:**							|**Formula:								|**

| Bug Leakage = (Production Defects / Total Defects) × 100	|Defect Density = Total Defects / Size of Module (LOC or Function Points)|



**| Entry Criteria | Exit Criteria         |**

**| -------------- | --------------------- |**

| Before testing | After testing         |

| Preconditions  | Completion conditions |

Entry criteria define when testing can start, and exit criteria define when testing can be completed.



**V-Model**

V-Model is an extension of Waterfall where **testing is planned parallel to development**.

**Structure**

Left Side → Development

Right Side → Testing

**| Development Phase | Corresponding Testing Phase |**

**| ----------------- | --------------------------- |**

| Requirement       | Acceptance Testing          |

| System Design     | System Testing              |

| High-Level Design | Integration Testing         |

| Low-Level Design  | Unit Testing                |

Testing activities are planned early.

In V-Model, testing is performed parallel to development phases, ensuring early defect detection and better quality control.



**Risk-Based Testing-** Testing approach where more focus is given to high-risk areas.

Example:

Payment module → High Risk → More testing

Static content page → Low Risk → Less testing

**Risk Factors:**

Business impact

Complexity

Integration dependency

Security concerns

In risk-based testing, we prioritize testing efforts based on business impact and criticality to ensure high-risk modules are thoroughly validated.







