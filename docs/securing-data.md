# Securing Data

Regulations, laws and good customer relationships mean it is essential to secure any
Personally identifiable information (PII). PII is any information connected to a specific individual that can be used to
uncover that individual's identity, such as their social security number, full name, date of birth or email address.
In the UK and EU these responsibilities are legally defined in the 2016 General Data Protection Regulation, normally
referred to as GDPR.

The website and apps secure data in the following way.

* Local storage (cookies for websites, app data for mobile apps) is limited to functional data (i.e. stored logins,
  remembering the current navigation).
* All data transmitted over the internet is secured using the standard secure https protocol
* Data is stored only on secure cloud managed database (*currently AWS but may change*)
* All applications credential are stored in an encrypted secret store (*currently AWS but may change*)
* All cloud administration requires hardware token authorisation (https://www.yubico.com/products/yubikey-fips/)  
* Each club has its own encrypted vault (todo , explain )