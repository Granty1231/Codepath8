# Project 8 - Pentesting Live Targets

Time spent: **3** hours spent in total

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

Vulnerability #1: SQL Injection (SQLi)
-allowed for sql sleep function

<img src=https://github.com/Granty1231/Codepath8/blob/master/cpweek8-sqli.gif/>

Vulnerability #2: Session Hijacking/Fixation
-allowed change of session id to hijack admin session

<img src=https://github.com/Granty1231/Codepath8/blob/master/cpweek8-session.gif/>

## Green

Vulnerability #1: Cross-Site Scripting (XSS)
-allowed for xss through the contact form

<img src=https://github.com/Granty1231/Codepath8/blob/master/cpweek8-xss.gif/>

Vulnerability #2: Username Enumeration
-bolded known users, unbolded unknown

<img src=https://github.com/Granty1231/Codepath8/blob/master/cpweek8-uenum.gif/>


## Red

Vulnerability #1: Insecure Direct Object Reference (IDOR)
-could access salespeople pages that were not public

<img src=https://github.com/Granty1231/Codepath8/blob/master/cpweek8-idor.gif/>

Vulnerability #2: Cross-Site Request Forgery (CSRF)
-could change the csrf token and still process changes

<img src=https://github.com/Granty1231/Codepath8/blob/master/cpweek8-csrf.gif/>


## Notes

- Syntax difficulties were hard, for example for SQLi, knowing where the vulnerability had to be: the URL still didn't allow me to know waht exact sql statement would be allowed.

- Challenges in finding/isolating these vulnerabilities on a large attack surface, took a while to locate.

