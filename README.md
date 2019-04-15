# Web-Security-Week-9 Pentesting Live Targets

Time spent: 5 hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:
* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)

## Blue

Vulnerability #1 - SQL Injection (SQLi):  <br />
* In "salesperson" page, SLEEP command is injected to the database. 
GIF Walkthrough: <br />
<img src="https://github.com/sengfung27/Web-Security-Week-9/blob/master/sqli.gif" width="800">

Vulnerability #2 -  Session Hijacking/Fixation:  <br />
* Attackers can reuse the session id after login on other browser as logged in user.
GIF Walkthrough: <br />
<img src="https://github.com/sengfung27/Web-Security-Week-9/blob/master/session-hijacking.gif" width="700">
