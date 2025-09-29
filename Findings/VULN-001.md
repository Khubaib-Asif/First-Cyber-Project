\# VULN-001 — SQL Injection (tautology) on DVWA (Low)



\*\*ID:\*\* VULN-001  

\*\*Target:\*\* DVWA on Metasploitable2 VM  

\*\*VM IP used during test:\*\* (e.g.10.0.0.5) 

\*\*Date:\*\* 2025-09-29



\## Summary

On DVWA's SQL Injection page (security: low), crafted input changed the WHERE clause and returned multiple user rows instead of a single row, demonstrating a SQL injection vulnerability.



\## Steps performed (safe — on isolated lab only)

1\. Boot Metasploitable2 and note the IP (example: `10.0.0.5`).  

2\. From host browser open `http://10.0.0.5/dvwa/`.  

3\. Login with `admin` / `password`.  

4\. Set DVWA security to \*\*low\*\*.  

5\. Navigate to \*\*SQL Injection\*\*.  

6\. Enter the payload: `1' OR '1'='1' #` and submit.  

7\. Observe multiple rows returned (proof of injection).



\## Evidence

\- `media/screenshot\_homepage.png` — DVWA app list.  

\- `media/screenshot\_security\_low.png` — DVWA security set to low.  

\- `media/screenshot\_sqli\_input.png` — the payload in the form.  

\- `media/screenshot\_sqli\_result.png` — results showing multiple rows.



\## Impact

An attacker with access to the web app could read data from the database, potentially exposing user credentials and other sensitive information.



\## Remediation

\- Use parameterized queries (prepared statements).  

\- Validate and sanitize inputs server-side.  

\- Use least-privilege database accounts for the web application.



