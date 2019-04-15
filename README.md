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
<img src="https://github.com/sengfung27/Web-Security-Week-9/blob/master/session-hijacking.gif" width="800">

## Green

Vulnerability #1 - Username Enumeration: <br />
* "Login was unsuccessful" is bold if username appeared in the database
GIF Walkthrough: <br />
<img src="https://github.com/sengfung27/Web-Security-Week-9/blob/master/user-enumeration.gif" width="800">

Vulnerability #2 - Cross-Site Scripting (XSS): <br />
* Attackers can perform xss under feedback section. In this example: \<script\>alert('xss');\</script\> <br />
GIF Walkthrough: <br />
<img src="https://github.com/sengfung27/Web-Security-Week-9/blob/master/xss.gif" width="800">

## Red

Vulnerability #1 - Insecure Direct Object Reference (IDOR): <br />
* Search salesperson by changing ID under the salesperson page: https://35.184.88.145/red/public/salesperson.php?id=X.
  
GIF Walkthrough: <br />
<img src="https://github.com/sengfung27/Web-Security-Week-9/blob/master/idor.gif" width="800">

Vulnerability #2 -  Cross-Site Request Forgery (CSRF)
* Attacker can design a form which would automatically submit form data to the staff area and take advantage of a logged in user's access permissions.
GIF Walkthrough: <br />
<img src="https://github.com/sengfung27/Web-Security-Week-9/blob/master/csrf.gif" width="800">



