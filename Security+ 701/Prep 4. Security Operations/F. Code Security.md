**Code Review** - software is one of the most common sources of security vulnerabilities
- *Code* - use peer analysis to assess code
- *Fagan Inspections* - follow a formalized, six-step code review process
	- The planning phase includes preparing materials, identifying participants, and scheduling the review
	- The overview phase includes assigning roles to participants and providing an overview of the software
	- During the preparation phase, participants independently examine the code for potential defects
	- During the inspection meeting, reviewers discuss and formally identify any code defects
	- During the rework phase, the code developers correct any defects identified during the inspection
	- During the follow-up phase, the leader verifies that defects were resolved and completes project documentation
Most organizations use a less formal review process

**Software Testing** - software testing ensures that finished code functions properly
- Verification and Validation:
	1. *Software Model Validation* - are we building the right software?
	2. *Software Verification* - are we building the software right?
- *Stress Testing* - uses automated scripts to verify system capacity, may be run internally or through a vendor, verifies the system can handle the maximum expected load, determines the maximum capacity of the system
- *User Acceptance Testing (UAT)* - ensures software will work for users, UAT is commonly referred to as "beta testing"
- *Regression Testing* - checks for unexpected side effects

**Code Security Tests** - code security testing checks software for application security flaws
- *Code Security Tests* - use technology to inspect software
	- *Static Tests* - use automated techniques to analyze code for errors and security flaws without actually executing it
	- *Dynamic Tests* - execute code to verify that it is functioning correctly and doesn't have security flaws
- *Synthetic Transactions* - supply input to code with known, expected outputs
Code reviews, static testing, and dynamic testing are complementary, rather than competitors

**Fuzz Testing**
- *Fuzzing* - fuzzing is a software testing technique that feeds software many different input values in an attempt to cause an unpredictable state or unauthorized access
	- Fuzz Testing Input Sources:
		- Developer-supplied input
		- Developer-supplied script
		- Generation fuzzing
		- Mutation fuzzing
	Avoid looking like a hacker, only fuzz test with permission

**Acquired Software**
- *Commercial Off-the-Shelf (COTS)* - purchased from third-party vendors and run on systems managed by the customer
- *Software as a Service* - software developed by vendors that run in the cloud on vendor-managed services
- Apply Vendor Security Updates:
	- Security patches
	- Hotfixes
	- Critical updates
	- Major and minor releases
Open-source software also requires careful management
- Configure Software Security:
	- Manage user accounts
	- Set administrative privileges
	- Deploy IP range restrictions

**Package Monitoring** - developers use third-party libraries and packages to save time, but that code may have security issues
- *Package Monitoring* - tracks third-party code, automated tools assist with package monitoring
Code from untrusted sources may introduce application vulnerabilities