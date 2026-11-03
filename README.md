# Loan Account Payment Calculator

A Java class that models a loan and calculates its **monthly payment** for different terms and interest rates, using the standard amortisation formula.

## How it works

```
monthly payment = principal × r / (1 − (1 + r)^−n)

r = annual interest rate / 12   (monthly rate)
n = number of monthly payments
```

`LoanAccount` keeps each loan's **principal** as private instance data, and the **annual interest rate as a static field** shared by every loan. Changing the rate once with `setAnnualInterestRate` updates the payments for all loans, which shows the difference between class-level and object-level state.

## Example output

Two loans, $5,000 and $31,000, over 3, 5 and 6 years, first at 1% and then at 5% interest:

```
Monthly payment for loan1 of $5000.00 and loan2 $31000.00 for 3,5, and 6 year loans at 1% interest.
Loan    3 years  5 years  6 years
Loan1   141.04   85.47    71.58
Loan2   874.45   529.91   443.78

Monthly payment for loan1 of $5000.00 and loan2 $31000.00 for 3,5, and 6 year loans at 5% interest.
Loan    3 years  5 years  6 years
Loan1   149.85   94.36    80.52
Loan2   929.10   585.01   499.25
```

## Run it

```bash
javac LoanAccount.java
java LoanAccount
```

The NetBeans project is also included as `Loan Account.zip`.

This is the first in a series of loan programs: [Loan Account Hierarchy](https://github.com/tisyavaidya/Loan-Account-Hierarchy) adds loan types through inheritance, and [Customer Loan Accounts](https://github.com/tisyavaidya/Customer-Loan-Accounts) adds customers with multiple loans. Coursework for a Java object-oriented programming course at Penn State.

## Tools

Java

---

[Tisya Vaidya](https://tisyavaidya.com) · [LinkedIn](https://www.linkedin.com/in/tisya-vaidya/) · [GitHub](https://github.com/tisyavaidya)
