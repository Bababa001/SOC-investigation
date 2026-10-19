SOC Investigation 001: Repeated Failed Login Attempts

1. Incident Overview

Incident Type: Suspicious Login Activity
Severity: Medium
Status: Investigated — Simulated Scenario
Analyst: Beginner SOC Analyst

2. Scenario

A simulated security log shows repeated failed login attempts against a user account within a short period. This activity may indicate a brute-force attempt, a forgotten password, or a misconfigured application.

3. Sample Log Evidence

The following entries are fictional examples created for training purposes.

Timestamp (UTC)	Source IP	Username	Event
09:00:01	192.0.2.10	user01	Login failed
09:00:05	192.0.2.10	user01	Login failed
09:00:09	192.0.2.10	user01	Login failed
09:00:13	192.0.2.10	user01	Login failed
09:00:17	192.0.2.10	user01	Login failed

Note: The IP address belongs to a range reserved for documentation and examples. These are not real incident logs.

4. Analysis

* Five failed login attempts occurred within approximately 16 seconds.
* All attempts originated from the same example IP address.
* All attempts targeted the same example account.
* The repeated pattern could indicate a brute-force attempt, but the evidence alone does not prove malicious activity.
* No successful login is shown in the supplied sample.

5. Risk Assessment

Potential Risk: An attacker could gain unauthorised access if the activity continues and valid credentials are discovered.

Assessment: Medium, pending further investigation. Severity may increase if a successful login, privileged account, or other suspicious activity is identified.

6. Recommended Actions

1. Check surrounding authentication logs for successful logins and related activity.
2. Determine whether the activity matches the user’s normal behaviour.
3. Review account lockout policies and multi-factor authentication status.
4. Apply approved rate-limiting or account protection controls if warranted.
5. Escalate according to the organisation’s incident response procedures if evidence of compromise emerges.

7. Conclusion

The simulated logs show repeated failed authentication attempts against one account. This pattern warrants further investigation but is not sufficient on its own to confirm a brute-force attack or account compromise.

8. Skills Practised

* Reviewing authentication logs
* Identifying repeated failed logins
* Assessing security risk
* Recommending defensive actions
* Documenting investigation findings

Training disclaimer: This report uses fictional data for educational purposes only.
