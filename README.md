# regex
List of common &amp; useful regex

## Numbers

- ``` ^\d+$ ``` - Positive
- ``` ^-\d+$ ``` - Negative
- ```  ^-?\d+$ ``` - Integer
- ``` ^-?\d*\.?\d+$ ``` - Pos/Neg
- ``` ^\+?[\d\s]{3,}$ ``` - Phone Number
- ``` ^(19|20)\d{2}$ ``` - 1900-2099
- ```^(\d|[1-9]\d|1\d\d|2[0-4]\d|25[0-5])\.(\d|[1-9]\d|1\d\d|2[0-4]\d|25[0-5]){3}$``` - IPV4 Address


## Alphabetic input

- ```^[\w.']{2,}(\s[\w.']{2,})+$ ``` - Full Name
- ``` ^[\w\d_.]{4,}$ ``` - Username
- ```^[_]*([a-z0-9]+(\.|_*)?)+@([a-z][a-z0-9-]+(\.|-*\.))+[a-z]{2,6}$``` - Email
- ```^([a-z][a-z0-9-]+(\.|-*\.))+[a-z]{2,6}$``` - Domain

## Passwords

- ```  ^.{6,}$ ``` - Password (min - 6 char)
- ```^[a-z0-9\.@#\$%&]+$ ``` - only contains letter [a-z] digits[0-9] and special characters(@#$%&)
- ```^(?=.*[A-Za-z])(?=.*\d)[A-Za-z\d]{8,}$  ``` - minimum 8 characters at least 1 letter and 1 number

- ```^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[$@$!%*?&])[A-Za-z\d$@$!%*?&]{8,}``` - minimum 8 characters at least 1 uppercase letter, 1 lowercase letter, 1 number and 1 special character


## Misc

- ```[A-Z]{1,2}[0-9][0-9A-Z]?\s?[0-9][A-Z]{2} ``` - UK Postcode
- ```^(\+44\s?7\d{3}|\(?07\d{3}\)?)\s?\d{3}\s?\d{3}$ ``` - UK mobile (+44 accepted)
- ```^([a-f0-9]{6}|[a-f0-9]{3})$ ``` - Hex Colour
- ```(?<Current>^[A-Z]{2}[0-9]{2}[A-Z]{3}$)|(?<Prefix>^[A-Z][0-9]{1,3}[A-Z]{3}$)|(?<Suffix>^[A-Z]{3}[0-9]{1,3}[A-Z]$)|(?<DatelessLongNumberPrefix>^[0-9]{1,4}[A-Z]{1,2}$)|(?<DatelessShortNumberPrefix>^[0-9]{1,3}[A-Z]{1,3}$)|(?<DatelessLongNumberSuffix>^[A-Z]{1,2}[0-9]{1,4}$)|(?<DatelessShortNumberSufix>^[A-Z]{1,3}[0-9]{1,3}$)``` - UK Number Plate

