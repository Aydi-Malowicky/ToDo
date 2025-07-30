const { test, expect, selectors } = require('@playwright/test');

    test("fill the form", async ({ page }) => {
    // Navigate to the initial URL
    await page.goto("https://forms.monday.com/forms/6912bb8ced0b4a3ebaf8e4cbbfaf8dfa?r=euc1");
    page.getByRole('textbox', { name: 'what would you like to buy?' }).fill('Laptop')
selectors.setTestIdAttribute('data-testid');
page.getByTestId('checkbox-checkbox_boolean_mknp4nba-checkbox').click()
page.getByRole('spinbutton', { name: 'how many would you like to order?' }).fill('1')
page.getByRole('textbox', { name: 'full name' }).fill('John Doe')
page.getByRole('button', { name: 'submit' }).click()
    });
    