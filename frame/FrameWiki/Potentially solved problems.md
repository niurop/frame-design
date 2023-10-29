**PROBLEM**(User identification):
How should users be identified.

**POTENTIAL SOLUTION**(User identification):
Users could be identified by a 64 bit `UUID` (Universally Unique Identifier).
Then each id have an account with increasing levels of identification:
- anonymous = \<login data\> {password; email} (should email be necessary)
- nicknamed = \<anonymous\> + \<nick\>
- named = \<nicknamed\> + \<full name\>
- associated = \<named\> + \<association\>
- KYC = \<associated\> + \<KYC\>