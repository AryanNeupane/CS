API Test Report- lEC

Date: 27/11/2082
API Base URL:https://lec-backend-gva9.onrender.com
Tested by: Aryan Neupane
Test Date: 27/11/2082
Test Report Submitted on: 27/11/2082
Module: Testing API
Test Priority: High
Test Type: Functional + Security
Submitted to: Sandeep Chalise

Pre-requirements

API server running and accessible
Valid test user credentials available
Postman
Stable internet connection

Platforms / Tools Used
Postman (Windows 11)


Detailed Test Cases
Test Case ID	Test Case	Expected Result	Actual Result	Status	Comments
TC_01	Verify username and password fields are mandatory	Request rejected with 400 — username and password missing.	400 error — username missing and password too short.	✅ Pass	Validations working properly.
TC_02	Verify login with valid credentials	Login successful; token and user info returned.	Login successful; user info and token provided.	✅ Pass	Working as expected.
TC_03	Verify login with invalid password	401 error — invalid credentials.	Login failed — invalid credentials.	✅ Pass	Correct error response.
TC_04	Verify login with invalid username	401 error — invalid credentials.	Login failed — invalid credentials.	✅ Pass	Working as expected.
TC_05	Verify login with invalid username & password	401 Unauthorized — both invalid.	Login failed — invalid credentials.	✅ Pass	Expected behavior.
TC_06	Verify login with empty username	400 error — username is required.	400 error — username is required.	✅ Pass	Validation correct.
TC_07	Verify very long username input	400 error — username too long.	400 error — username length is invalid.	✅ Pass	Working properly.
TC_08	Verify very long password input	400 error — password too long.	400 error — password length is invalid.	✅ Pass	Boundary validation OK.
TC_09	Verify login attempt rate limit	429 error — too many attempts.	Login blocked — too many attempts.	✅ Pass	Rate-limit functioning.
TC_10	Verify trimming spaces in username	Login successful; user info + token.	Login successful; token generated.	✅ Pass	Trimming works.
TC_11	Verify username case sensitivity	Login should work regardless of case sensitivity.	Login successful; token generated.	✅ Pass	Case-insensitive login.
TC_12	Verify password case sensitivity	401 error — wrong case should fail.	Login failed — invalid credentials.	✅ Pass	Password is case-sensitive.
TC_13	Verify incorrect endpoint	Should show 404 Not Found	Returns 401 Unauthorized	❌ Fail	Wrong status code handling.
TC_14	Verify wrong HTTP method (GET)	405 error — method not supported.	405 error — method not supported.	✅ Pass	Correct method validation.
TC_15	Verify account lock mechanism	423 error — locked after multiple failures.	423 error — account locked.	✅ Pass	Lockout feature works.
TC_16	Verify no sensitive info leaked in errors	401 error — generic message.	401 error — invalid credentials.	✅ Pass	No data leakage.
TC_17	Verify different Content-Types (non-JSON)	415 error — unsupported media type.	400 error — unsupported Content-Type.	⚠️ Partial Pass	Status code mismatch.
TC_18	Verify login with special characters	401 error — invalid creds.	401 Unauthorized — invalid creds.	✅ Pass	Correct rejection.
TC_19	Verify login response headers	content-type: application/json + cache-control: no-store present	Same headers returned	✅ Pass	Correct headers.
TC_20	Verify successful login returns valid JWT	Should return correct payload (role + exp).	Returns correct data.	✅ Pass	Token valid.


Post-Conditions

Login endpoint functioning with proper validations.
Rate limit & lockout mechanisms work correctly.




Prepared by: Aryan Neupane
Submitted to: Sandeep Chalise
Date: 27/11/2082