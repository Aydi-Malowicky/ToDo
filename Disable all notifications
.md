const { test, expect, selectors } = require('@playwright/test');

    test("Disable all notifications
", async ({ page }) => {
    // Navigate to the initial URL
    await page.goto("https://app.uat.spontivly.com/ui/dashboard/home");
    page.getByRole('textbox', { name: 'you@example.com' }).fill('tom.brachel@tutoit.io')
page.locator("css=[type='password']").fill('Tomb2411')
page.getByRole('button', { name: 'log in' }).click()
page.locator("css=.css\-f63w6y").filter({ hasText: 'organization settings' }).click()
page.getByRole('button', { name: 'notifications' }).click()
page.locator("css=.w\-full.rounded\-md").locator("css=.flex").filter({ hasText: 'all notificationstoggle all notifications' }).getByRole('checkbox').click()
page.getByRole('button', { name: 'confirm' }).click()
page.locator("css=.w\-full.rounded\-md").locator("css=.flex").filter({ hasText: 'all notificationstoggle all notifications' }).getByRole('checkbox').click()
page.getByRole('button', { name: 'confirm' }).click()
    });
    