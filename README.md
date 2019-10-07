# Quality Assurance Engineer Take Home Exam

Quality Assurance Screening Project

## Instructions
This is the take home exam for QA Engineer candidates of Digix Global. In order to pass the exam, you must accomplish the following:
- Fork this repository and create a Pull Request with the changes described in the task list below. Some tasks are optional, but doing them will greatly improve the prospects of you being hired.
- Answer the questionnaire below. These questions are open-ended and are intended for us to gauge your current skill level in automation scripting.
- Script should be able to run on chrome and firefox browsers
- Test scripts should generate a test report
- Create an `INSTRUCTION.md` file how to setup the environment and how to run the test. 
- Create also a Pull Request once you have finished the exam

You have five (5) days to complete all tasks. If you finish one before the other, you may send them earlier. If you wish to amend your submission for either requirement, you may do so as long as its within the five-day deadline. Best of luck!

## Requirement #1: Create us an end-to-end test suite that will do that following funnels
Test Environment: https://www-kovan.digixdev.com/app/#/marketplace/register
1. Signup 
2. Email verification
3. Login 
4. Log the userAgent on the test report

**Note: test can be run multiple times without any issues on signup**

## Requirement #2: Create us a test suite that will  do the 1st step of KYC(Basic Info)
Test Environment: https://www-kovan.digixdev.com/app/#/marketplace/
- Steps:
  1. Login the account (use credentials below)
  2. Go to KYC page by clicking the email address on top right then select account
  3. Click "Submit KYC Information" button
  4. Fill in Basic Info Form (first Name, last Name, Date of Birth, Gender, Phone Number, Nationality)
  5. Paste `0xAf570b855366136799697a2bcB99002de3c092a6` to Markeplace Ethereum Address field
  6. Click "Next Step" button
  7. Assert "Country of Residence" dropdown
```      
   login credentials: 
      - email: digixtemail+exam@gmail.com
      - password: test1234
 ```
 ## Requirement #3: Create a test suite that will do comprehensive test on Login funnel (Use credentials below for your valid output)
Test Environment: https://www-kovan.digixdev.com/app/#/marketplace/
```
   login credentials: 
      - email: digixtemail+exam@gmail.com
      - password: test1234
 ```
 
 ## OPTIONAL #4: Write a cron syntax that will run a script every 15 mins from 10am to 6pm Monday to Friday
