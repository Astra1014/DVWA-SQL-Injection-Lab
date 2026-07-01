# Findings

## Vulnerability

The SQL Injection module in DVWA intentionally demonstrates how an application can become vulnerable when user input is incorporated into SQL queries without proper protection.

## Observation

During testing, the application behaved differently when specially crafted input was supplied compared with ordinary input. This illustrates how insecure query construction can affect application behavior.

## Impact

If this type of vulnerability existed in a production application, an attacker could potentially access or manipulate database information, bypass authentication, or retrieve sensitive records.

## Risk Level

High

## Recommended Mitigations

* Use prepared statements.
* Use parameterized SQL queries.
* Validate and sanitize user input.
* Apply least-privilege permissions to database accounts.
* Avoid exposing detailed database error messages.
* Perform regular secure code reviews and penetration testing.

## Conclusion

DVWA provides a safe environment for understanding SQL Injection vulnerabilities. The exercise reinforced the importance of secure coding techniques and proper database security controls to reduce the risk of SQL Injection attacks.
