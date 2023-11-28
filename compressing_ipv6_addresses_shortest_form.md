# COMPRESS AN IPV6 TO ITS SHORTEST FORM
IPV6 usually has 8 sections/parts (similar to Octets in IPV4 addresses) when in its longest form. Each Section usually has 4 letters, numbers or a combination of both. Each section is separated by a full colon

EXAMPLE IPV6 in Longest Form -  **1234:ABCD:4321:DCBA:2341:BACD:1342:ACBD** equivalent to  **SECTION1:SECTION2:SECTION3:SECTION4:SECTION5:SECTION6:SECTION7:SECTION8**

## IPv6 Compression rules:

## **1. Continuous 0s are replaced with ::**

Example 1- 0000:0000 becomes ::

Example 2- 0000:0000:0000 becomes ::

## **If there are 2 sets of continuous 0s in an IP address, only the first set gets replaced with ::. In the second set, one 0 should remain.**

Example- 3a09:0000:0000:1c2g:d77f:0000:0000:12ce becomes 3a09::1c2g:d77f:0:0:12ce

## **2. Remove leading 0s.**

Example 1- 0aed becomes aed

Example 2- 0046 becomes 46

## **if there are continuous zeros withot any values between them they can be replaced with ::**
Example 1 6fce:0000:0000:0000:0fff:abcd:907a:cd12 becomes 6fce::fff:abcd:907a:cd12

Example 2 6fce:0000:0000:0000:0000:0000:0000:cd12 becomes 6fce::cd12

Example 3 0000:0000:0000:0000:0000:0000:0000:0b12 becomes ::b12

