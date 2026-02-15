✅ Final Submission (Required Format)
🔹 Title

Secure API Testing and Authorization Validation

🔹 Objective

To evaluate the security of REST APIs by testing authentication mechanisms, authorization controls, input validation, and rate limiting.

🔹 Tools Used

Postman (API testing tool)

Sample REST API endpoints

Internet connection

🔹 Procedure

Configured API requests in Postman.

Tested API access with valid credentials.

Tested API access with invalid credentials.

Removed authentication headers and sent requests.

Modified resource identifiers to test authorization.

Sent malformed input data.

Sent multiple rapid requests to test rate limiting.

🔹 Observations

Valid credentials allowed access to API resources.

Invalid credentials returned “401 Unauthorized”.

Some endpoints responded even without authentication.

Changing resource IDs exposed data of other users.

API accepted malformed inputs without validation.

No restriction on rapid repeated requests.

🔹 Analysis

The API has multiple security weaknesses:

Missing authentication on some endpoints

Broken authorization (access to other users’ data)

Weak input validation

Absence of rate limiting

These vulnerabilities could lead to data breaches and service abuse.

🔹 Result

Critical vulnerabilities were identified, particularly broken authorization and improper access control mechanisms.

🔹 Conclusion

Secure API design requires strong authentication, proper authorization checks, input validation, and rate limiting. Addressing these issues is essential to protect sensitive data and ensure system integrity.
