### Repository Overview

This repository contains the test case documentation for Kara David's Wish Note App, focusing on functional testing of the Data Entry page and backend validation using MySQL queries.

### Repository Contents

* Part A: Repository component A.

* Part B: Repository component B.

* Part C: Repository component C.

### Test Case Documentation

### Test Case Information

| Field           | Details                                                                                                                       |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| Test Case ID    | TC-DataEntry-001                                                                                                              |
| Test Case Title | Data Entry - Valid                                                                                                            |
| Application     | Kara David's Wish Note App                                                                                                    |
| Test Type       | Functional Testing                                                                                                            |
| Database        | birthday_wishnote                                                                                                             |
| Table           | main_corrupt_politicians                                                                                                      |
| Test Data       | Five valid entries containing First Name, Last Name, Government Position, and Location within their maximum character limits. |
| Status          | Pending Execution                                                                                                             |

### Preconditions

* Kara David's Wish Note App is running locally.

* The `birthday_wishnote` database and `main_corrupt_politicians` table exist.

* The Data Entry page is accessible using Chrome.

### Test Steps and Results

| Step | Action                                                                                                                               | Expected Result                                                                                                                                                                   | Actual Result                                                                            |
| ---- | ------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| a    | Verify that the form contains labels in the proper order and the text boxes are writable.                                            | The form displays the four labels in the correct order, and all text boxes are writable.                                                                                          | The form displays the four labels in the correct order, and all text boxes are writable. |
| b    | Verify the "Send Wish Note" button.                                                                                                  | The "Send Wish Note" button changes color on hover and is enabled.                                                                                                                | The "Send Wish Note" button changes color on hover and is enabled.                       |
| c    | Enter valid test data into the respective fields.                                                                                    | All fields accept valid test data within their character limits.                                                                                                                  | The fields accept valid test data.                                                       |
| d    | Click "Send Wish Note" and verify that a modal appears.                                                                              | A verification modal appears after clicking "Send Wish Note".                                                                                                                     | Pending Execution                                                                        |
| e    | Verify that the modal contains the same information as the test data.                                                                | The modal displays the entered values correctly, including Location.                                                                                                              | Pending Execution                                                                        |
| f    | Click the Cancel button.                                                                                                             | The Cancel button closes the modal without submitting the form.                                                                                                                   | Pending Execution                                                                        |
| g    | Click "Send Wish Note" again and then click "Confirm & Send".                                                                        | Clicking "Confirm & Send" submits the form data.                                                                                                                                  | Pending Execution                                                                        |
| h    | Verify that a successful entry message appears on the Data Entry page.                                                               | A success message appears after successful submission.                                                                                                                            | Pending Execution                                                                        |
| i    | Verify the test data in the database using the following MySQL query: USE birthday_wishnote; SELECT * FROM main_corrupt_politicians; | The database contains the submitted First Name, Last Name, and Government Position. Location may be missing because the application intentionally omits it from the INSERT query. | Pending Execution                                                                        |

### Test Data and Database Validation

The test uses five valid entries containing First Name, Last Name, Government Position, and Location within their maximum character limits.

Execute the following MySQL query to verify the submitted records:

```sql
USE birthday_wishnote;
SELECT * FROM main_corrupt_politicians;
```

### Test Execution Status

* Steps a–c: Completed with the actual results documented above.

* Steps d–i: Pending execution. Results must be recorded after the corresponding tests are performed.

* Overall Status: Pending Execution — update to Passed or Failed after completing the test.

### Source Documentation

The original test case source file is named `textcase.txt`. Its test case details, expected results, actual results, and execution status are the basis for this document.
