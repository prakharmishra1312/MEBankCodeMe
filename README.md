# Munshi
# MEBankCodeMe

Design:
   The application has only one Class : com.mebank.accountoperation.AccountBalanceCalculator It has a functions:
   - setCSV: to set the CSV file with transactions 
   - calculateBalance: It takes the Account Id, from and to time as input strings and return a string output in this format:
    "Relative balance for the period is: "+balString+"\nNumber of transactions included is: "+transactions
    to Calculate the balance, the functions iterates the CSV records, and filters the records based on the time and the Account ID. An additional check is done for REVERSAL payment to roll back any eligible transactions.
    

Testing the application
  Run the test using maven:
  mvn -e -Dtest="com.mebank.test.**" test

  Run the test using Eclipse:
    Export the project
    Right click on the package com.mebank.test under /AccountBalanceCalculator/src/test/java and select Run as Junit test.

