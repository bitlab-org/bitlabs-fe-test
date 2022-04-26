# Introduction
This exercise will involve building a page for generating a quote for buying a specific cryptocoin.
A quote is a set of numbers that indicate how much money a customer will pay/receive, including the relevant fees.
Specifically, the page you need to build will be calculating how much USDC_EVMOS (a crypto coin) a customer will receive
in exchange for a specific amount of USD. The page will calculate this by making a request to a provided REST API.
You will not need to do any maths, only display the values you receive from the API.
The docs for the endpoint of interest are hosted at
https://api-qjoa5a5qtq-uc.a.run.app/redoc#operation/create_quote_quotes_post, the actual endpoint is
`POST https://api-qjoa5a5qtq-uc.a.run.app/quotes`. You do not need to worry about the quote expiring in this exercise.

### Detailed exercise specification
- You need to build a page in React that resembles the design presented here - **FIGMA LINK HERE**.
  **Initially, do not worry about CSS/design and get the functionality working first.**
- The page should allow the client to enter **either** the source USD amount **or** the target USDC_EVMOS amount.
  Upon changing **either** of these amounts the page should make a request to the API to generate a quote with
  the newly-entered value.
  
  The API supports generating a quote either using the source amount (USD) or the target amount (USDC_EVMOS),
  please refer to the documentation of the API for more information.
- We expect you to have at least some basic tests for your React code. Tests should be runnable using 
  the `yarn test` command.
#### Bonus Points
- Once you have the functionality working, you should try to get the design resemble the figma provided.
- If you manage to get all of the above working, implement a spinner that should show while the front-end is
  waiting on the REST API to respond.

# Project Contents

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.
