ASSURITY TECHNICAL ASSESSMENT


[CONTEXT]
Using the API given below create an automated test with the listed acceptance criteria:
API = https://api.tmsandbox.co.nz/v1/Categories/6327/Details.json?catalogue=false
 

Acceptance Criteria:

(01) Name = "Carbon credits"
(02) CanRelist = true
(03) The Promotions element with Name = "Gallery" has a Description that contains the text "Good position in category"


[INSTRUCTIONS]

(01) Your test needs to be written using a programming language of your choice (not a tool like SoapUI or a DSL based tool like robot framework) we want to see how you code! Ensure you include a clear ReadMe

(02) Submit your test to us in a format that lets us execute and review the code (it must be submitted in a public repository like Bitbucket or Github)

(03) Your test must validate all the three acceptance criteria

(04) Points will be awarded for meeting the criteria, style and the use of good practices and appropriate use of source control

(05) We want to see your best work - no lazy coding or comments.

[TESTS]

There are two GET request created for this exercise:

(01) Random Generated Category 
I use a variable in the provided API to hold random category numbers to pull in and validate.
In the Pre-request, I put a JSON code to generate a number and saved in the variable.


(02) Carbon Credits Category
I use the provided API as is as baseline as the three acceptance criteria are met.



For each request, I use JSON script to run the following tests:

(01) response has the right status code
(02) response body contains "Carbon credits" category name
(03) response body contains Relist boolean as TRUE
(04) response body contents Promotions element with Name as Gallery

