# Spring-Security-Day4



DelegatingPasswordEncoder the general format for a password is: {id}encodedPassword

Such that id is an identifier used to look up which PasswordEncoder should be used and encodedPassword is the original encoded password for the selected PasswordEncoder. 
The id must be at the beginning of the password, start with { and end with }. 
If the id cannot be found, the id will be null. For example, the following might be a list of passwords encoded using different id. All of the original passwords are "password".



Id examples are:

{bcrypt}$2a$10$dXJ3SW6G7P50lGmMkkmwe.20cQQubK3.HZWzG3YB1tlRy.fqvM/BG {noop}password

{pbkdf2}5d923b44a6d129f3ddf3e3c8d29412723dcbde72445e8ef6bf3b508fbf17fa4ed4d6b99ca763d8dc 

{scrypt}$e0801$8bWJaSu2IKSn9Z9kM+TPXfOc/9bdYSrN1oD9qfVThWEwdRTnO7re7Ei+fUZRJ68k9lTyuTeUp4of4g24hHnazw==$OAOec05+bXxvuu/1qZ6NUR+xQYvYv7BeL1QxwRpY5Pc=

{sha256}97cde38028ad898ebc02e690819fa220e88c62e0699403e94fff291cfffaf8410849f27605abcbc0




create bcrypt password

https://www.browserling.com/tools/bcrypt
