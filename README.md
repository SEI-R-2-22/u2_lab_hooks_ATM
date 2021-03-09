# React Hooks ATM

![Bird](https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fwww.aestheticatms.com%2Fuploads%2F1%2F2%2F0%2F1%2F120178223%2Fmoney-bird_orig.gif&f=1&nofb=1)

## Overview
In this lab, we'll practice modifying an existing codebase. This repository contains the code for an existing ATM application using React. In it, you can currently deposit money into a checking account.

## Objectives
- Add the ability to withdraw money
- Add the ability to have a savings *and* checking account

## What You'll Be Building
![ATM](https://cloud.githubusercontent.com/assets/4304660/24376818/18c39a82-12f2-11e7-81e7-af618c22b3ed.png)

## Getting Started
- `fork` and `clone` to your machine
- `cd` into the directory
- `npm i` to install our dependencies
- `npm start` to spin up the app

## Your Task
Currently, you can see that there is a Checking account where a user can deposit money. Try it out - it already works!

We need to:
- Create a "Withdraw" button next to the "Deposit" button.
  - You ***should not*** be able to withdraw more than the current balance.
- Create a Savings account - another component of the same class.
  - It will have the same deposit (and eventual withdraw) functionality.
- You ***should not be able*** to type negative numbers into either withdraw or deposit.

### Hints
<details>
<summary>Stuck on making a Savings account? Here's a hint:</summary>
The <code>name</code> prop being passed into <code>Account</code> is "Checking" - perhaps you can just call the component again for "Savings".   
</details>

<details>
<summary>Stuck on making a Withdraw button? Here's a hint:</summary>
Functionality to withdraw money is quite similar to functionality for depositing money, except with subtraction instead of addition.
</details>

<details>
<summary>Stuck on limiting negative numbers? Here's a hint:</summary>
When a function checks if the input is a number (with <code>isNaN</code>), an <code>||</code> condition could be added to be sure the input is not less than 0.
</details>
