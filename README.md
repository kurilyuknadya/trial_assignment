# trial_assignment
Here is my first attempt to perform possible interview tasks

ASSIGNMENT

   You need to check the registration form on the website of the online store.
1) Identify as many tests as possible that need to be conducted.
2) Write at least five test cases.
Specification
The user has to fill in the required data in order to get access, as a standard user.
At this time, only the First Name, Last Name, and E-mail address fields can be checked. The maximum length of each field is 30.

ANSWER

First, I figured out what methods or approaches to use.

Technics that I will use:
boundary value analysis,
scenario testing,
security,
domain testing,
technology.

From a boundary value analysis:
less than minimum value (empty value or space),
minimum value(one single char, unless otherwise specified in the specification, I think it may be so),
maximum value(we have in specification 30 characters),
more than maximum value(31 characters).

From a scenario perspective:
in the First and Last Name should not be any spaces (space values at the beginning, at the end, in the middle),
check used HTML tags (<h>text</h>),
same e-mail address,
wrong e-mail address,
“nasty words”.

From a security perspective: 
basic SQL ingection(so values as single qoute ( ‘ ) or semicolon ( ; )),
cross site scripting (XSS) (<script></script>)
extremely big requests.

Domain testing perspective:
other characters than alfabetic(! # % ; { $ & *),
average value (between 1 and 30).

Technology perspective:
non ASCII ( µ₦؄₿℥),
check the page source,
check missing CSS
look at the cookie.

Usability testing:
tab navigation,
different browsers, 
browser zoom in and out.
 First of all, I will perform a positive test, use the correct data.


