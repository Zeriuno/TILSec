--- 
title: Why your password can’t have symbols—or be longer than 16 characters
url-text: https://arstechnica.com/security/2013/04/why-your-password-cant-have-symbols-or-be-longer-than-16-characters/
date-card: 2017-01-30
date-text: 2013-04-29
tags: 
- password
---

As Thomas Baekdal wrote back in 2007, a password that’s just a series of words can be “both highly secure and user-friendly.” But this scheme, as well as other password design tropes like using symbols for complexity, does not pass muster at many sites that specify an upper limit for password length.

## Examples

* Financial company Charles Schwab: 6 < password < 8 (in fact they allow more, but they are truncating!)
* Microsoft: 8 < password < 16
* Evernote: 6 < password < 64; spaces not allowed
* AT&T: 8 < password < 64; no symbols except `_-`
* Capital One: 8 < password < 15; no symbols except `_-`

### Exlpanations

The reason for short password length requirements is because they don't believe that their systems will be hacked. Short passwords are only a security problem if the hash lists are obtained. If you believe your system is impenetrable, you only have to worry about user failures -- phishing and the like -- and long or complicated passwords really make no difference in those cases.

Microsoft declares that the most important threat are phishing, compromised machines and password reusing, not password cracking (the situation is changing) and accounts can't be defended by password lenght.
Password validation is decentralized across different products, hence hard to change (legacy, which is more common than admitted), whereas some cricisists think Microsoft might be storing plain-text password instead of hashing them.

Evernote says that some UI frameworks and third-party applications would trim leading and trailing spaces. Adding support for spaces only in the middle of the password would make the regular expression defining them three times longer and would increase the enthropy of only 1.5%

AT&T told users do not like to type spaces on mobiles, and some words (profanities) are forebidden


## Sources

* Thomas Baekdal's 2007 text: http://www.baekdal.com/insights/password-security-usability
* Easy bypassing of security questions: http://www.theatlantic.com/technology/archive/2012/08/security-questions-the-biggest-joke-in-online-identity-verification/260835/
* About password cracking: http://arstechnica.com/security/2013/03/how-i-became-a-password-cracker/
* Stackoverflow thread discussing Microsoft's explanation: http://stackoverflow.com/questions/98768/should-i-impose-a-maximum-length-on-passwords
* Profanities unallowed in passwords: http://arstechnica.com/security/2013/04/wtf-ats-profane-password-ban-lets-some-swears-through/
* advances in cracking passwords: http://arstechnica.com/security/2012/08/passwords-under-assault/