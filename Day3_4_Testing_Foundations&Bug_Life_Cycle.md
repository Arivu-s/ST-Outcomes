**Day 3 – Testing Foundations**

** **

**1. Test Plan ➝ 2. Test Scenarios ➝ 3. Test Cases ➝ 4. Test Data ➝ 5. Test Suite**



**Term		What it Represents	  Document		Example							Tool			People**

Test Plan	Overall testing strategy  .docx/.pdf		Document detailing scope, schedule, tools, risks	Word, Confluence	Test Lead

Test Scenario	What to test		  .xlsx			"Check login with valid credentials"			Excel, TestRail		QA Engineer, BA

Test Case	Steps to test		  .xlsx or Test Tool	"Enter username, password, click login"			Excel, Zephyr, TestLink	QA Engineer

Test Data	Input values for testing  .xlsx or inline	Username: testuser, Password: Test@123			Excel, DB, Postman	QA + Developer

Test Suite	Group of test cases	  Grouped in tool	"Authentication Tests"					TestRail, Excel		QA Engineer



**Day-4 Defect Life cycle**



Defect/ Bug Life cycle is the journey of the defect from the moment it is identified to until it is closed.



**Status of Defect Life Cycle**

The flow of the bug life cycle will be as follows:



New-->Assigned-->Open-->Fixed-->Pending Retest-->Retest-->Verified-->Closed

 			    |			  |

 			   <-----------Reopened<--|(Not fixed)



These bugs, when identified, can be categorized or prioritized according to the severity and priority level(seriousness of the bug and how fast it to be closed).



&nbsp;      **\*\*Severity**				|		**Priority\*\***

1. How serious the defect is			|How urgently it needs to be fixed
2. It is decided by QA				|It is usually decided by PO
3. Categorized as Critical, major, minor	|Prioritized as High, Medium, Low



**Severity vs Priority Table**

**| Severity | Priority | Example                        |**

**| -------- | -------- | ------------------------------ |**

**|** High     | High     | Application crash              |

| High     | Low      | Rarely used feature failing    |

| Low      | High     | Company logo wrong on homepage |

| Low      | Low      | Minor UI misalignment          |



