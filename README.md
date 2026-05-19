# CSE 110 Lab 7

**Members**: Andre Lew

## Check Your Understanding

1. Where would you fit your automated tests in your Recipe project development pipeline? Select one of the following and explain why.

   I would put automated tests within a GitHub Action that runs whenever code is pushed. This is the best option because the tests would run automatically before new code is merged, meaning that bugs would be caught early without relying on everyone to remember to run tests locally. It also helps make sure the project still works as teammates add new features.

2. Would you use an end to end test to check if a function is returning the correct output? (yes/no)

   No, I would use a unit test for that. Unit tests are used to check small bits of code, like whether a function returns an expected output. End-to-end tests are better if you are testing something like a full user workflow through the website.

3. What is the difference between navigation and snapshot mode?

   Navigation mode analyzes the page right after it loads, as if a user just opened the URL. It's useful for checking overall initial page load performance. Snapshot mode analyzes the page in its current state, so it's better for checking things like accessibility issues after the page is already loaded. However, it can't measure JavaScript performance during load or track how the DOM changes over time.

4. Name three things we could do to improve the CSE 110 shop site based on the Lighthouse results.
   - Add a `lang` attribute to the `<html>` tag (`<html lang="en">`) to improve accessibility for screen readers
   - Add a meta description to the `<head>` to improve SEO and help search engines understand the page better
   - Reduce unused + minify JS to improve performance and decrease the amount of unnecessary code the page loads
