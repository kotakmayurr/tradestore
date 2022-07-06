# tradestore


##### Steps to run the code <H6>

Downlaod the repo.
Import the Java Project
go to maven (Right hand side menu) click on clean and install - it will run the test cases as well. you will be able to see in console logs.
Run the TradestoreApplication in com.db.tradestore (src/main)

  
##### Steps to execute test cases <H6>
  Runt the test case from src/test - TradestoreApplicationTests.java

###### Test Cases Output <H6>
- All test Case Passed.
  

# Problem statement

Write a Java program with all the JUNIT cases. TDD approach will be preferred. Time to complete the
below assignment is 1 hr.

Problem Statement
There is a scenario where thousands of trades are flowing into one store, assume any way of
transmission of trades. We need to create a one trade store, which stores the trade in the following
order

Trade Id Version Counter-Party Id Book-Id Maturity
Date

Created
Date

Expired

T1 1 CP-1 B1 20/05/2020 &lt;today
date&gt;
N
T2 2 CP-2 B1 20/05/2021 &lt;today
date&gt;
N
T2 1 CP-1 B1 20/05/2021 14/03/201
5

N
T3 3 CP-3 B2 20/05/2014 &lt;today
date&gt;
Y

There are couples of validation, we need to provide in the above assignment
1. During transmission if the lower version is being received by the store it will reject the trade and
throw an exception. If the version is same it will override the existing record.
2. Store should not allow the trade which has less maturity date then today date.
3. Store should automatically update the expire flag if in a store the trade crosses the maturity
date.
