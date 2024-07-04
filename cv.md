# Aleksandra Karlova

Senior QA Engineer

![Profile image](https://lh3.googleusercontent.com/a/ACg8ocJ1mCVio3TcX_Bx_ckqdA1zo0hp0QxLdMlG-Ot0m4_ogr7EtmRe=s288-c-no)

## Contacts

* **Location**: Berlin, Germany
* **Linkedin**: [https://www.linkedin.com/in/aleksandrakarlova/](https://www.linkedin.com/in/aleksandrakarlova/)
* **GitHub**: @AleksandraKarlova

## Summary
QA Engineer with more than 7 years of manual web and mobile testing experience in Fitness, Healthcare, E‑commerce and other areas, able to
lead testing process in distributed product teams.

I prioritize ongoing learning and growth, demonstrating a commitment to personal and professional development.

At work I actively contribute to streamlining testing processes to enhance the efficiency of the testing team.

## Skills

* **Python**: Basics
* **Java**: Basics
  * **Frameworks**: Selenium, Serenity BDD
* **JavaScript**: Basics
  * **Frameworks**: Cypress, Playwright
* **SQL**: Intermediate
* **Postman**: Intermediate
* **Charles Proxy**: Intermediate
* **Test Rail**: Intermediate
* **German Language**: Basic
* **English Language**: Advanced

## Code Examples

Auto-tests for Login functionality for [douglas.de](https://www.douglas.de/de/login)

```javascript
test.describe('Password Reset Test Suite', () => {

  test.beforeEach(async ({ page }) => {
    await page.goto('https://www.douglas.de/login');
    await page.getByRole('button', { name: 'Nur Unbedingt Erforderlich' }).click();
    await page.getByText('Passwort vergessen?').click();
  });
  
  test('Reset password with valid e-mail', async ({ page }) => {

    // Enter existing e-mail to reset password
    await page.getByRole('textbox', { name: 'E-Mail-Adresse*' }).click();
    await page.getByRole('textbox', { name: 'E-Mail-Adresse*' }).fill(testData.validUser.email);
    await expect(page.locator('#forgotPasswordForm').getByRole('img')).toBeVisible();

    // Click on Send E-mail button
    await page.getByRole('button', { name: 'E-Mail absenden' }).click();

    // Expect 'E-mail sent' dialog to be opened
    await expect(page.getByRole('heading', { name: 'E-Mail verschickt' })).toBeVisible();

    // Close the dialog
    await page.getByRole('button', { name: 'Schliessen' }).click();
  });
});
```

## Work Experience

### Spark Networks GmbH Berlin, Germany

#### QA ENGINEER (PAYMENTS, TRUST AND SAFETY) Jul 2022 ‑ Dec 2023

* Testing subscriptions on web, Android, and iOS platforms
* Testing payments made through Credit Card, PayPal, and the Google and Apple stores
* Testing mechanisms designed to prevent fraud on the app
* Analyzing fraudsters’ behavior patterns to identify new trends and prevent fraudulent attempts
* Improving testing approaches to enhance efficiency and accuracy

### SberMarket Moscow, Russia

#### QA ENGINEER / QA LEAD (ORDERS AND DiSPATCHiNG) May 2021 ‑ Jun 2022

* Manual API testing, UI testing, mobile testing (Android only)
* Improving testing processes within the teams
* Developing a testing strategy for the domain
* Mentoring and training new team members
* Recruiting and hiring new employees

### VTB Moscow, Russia

#### QA ENGINEER (B2B TRANSACTiONS) Nov 2020 ‑ Apr 2021

* Testing the application’s API to ensure smooth and secure transactions
* Verifying the usability and functionality of the application’s user interface
* Developing and maintaining test cases and test suites to document the testing process
* Running automated tests written by another QA and analyzing the results to identify and fix any issues

### Mercury Development Samara, Russia

#### QA ENGINEER / QA LEAD Jun 2016 ‑ Nov 2020

* Ensuring the functionality and performance of the web‑based services and mobile apps
* Verifying the usability and functionality of the user interface for all platforms
* Testing on iOS and Android platforms
* Developing and maintaining test plans and checklists to document the testing process
* Leading and mentoring a team of 2‑5 QA engineers
* Providing guidance and training to junior QA engineers
* Continuously working to improve testing processes and increase efficiency within the teams

## Education

Samara State University of Architecture and Civil Engineering  
Samara, Russia  
Sep 2007 ‑ Jun 2012  
M.A. in HEAT AND GAS SUPPLY AND VENTILATION
