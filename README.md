💰Expense-manager is a [progressive web application](https://developers.google.com/web/progressive-web-apps/) on top of [Google Sheets](https://developers.google.com/sheets/) 📉 written in [React](https://facebook.github.io/react/) ⚛️. It is only a static HTML that works great on mobile 📱 and can be deployed anywhere.


![Delete expense](doc/delete-expense.gif)

It was inspired & fork by the [expense](https://github.com/jakubgarfield/expenses) by jakubgarfield 

## Features

* Multiple accounts
  * Checking, savings, joint, etc.
* Categories
* [Google Sheet](https://docs.google.com/spreadsheets/d/1Lz1_gHIgCKPKhJpFerq9PoNy-TIst7eLZ5plQi5Prv0/edit?usp=sharing) as a backend

  * Uses Google Sheet as a database to store expenses. Why?
     Privacy. It's your personal data. It should belong to you.
     Sheets is way better at handling numbers than me. You can do all kinds of analysis using graphs, formulas, etc.
     I didn't want to write backend 🤓
     Unlimited analysis up to your sheet skill.
* Works great on mobile
  * Progressive Web App. Loads quickly and works as a standalone app.
* Beautiful material design
  * Better than native ;)
* Recurring expenses
  * Totally doable with [Zapier](http://zapier.com/).
* Monthly summary
  * This month. Last month. You immediately know how you doing.

## Get started

1) make a copy of [Expense Sheet](https://docs.google.com/spreadsheets/d/1Lz1_gHIgCKPKhJpFerq9PoNy-TIst7eLZ5plQi5Prv0/edit?usp=sharing) to your drive `File -> Make a copy...`
2) note the id of your new sheet (it's part of the URL)
3) clone, install dependencies and build the app:


```
npm i && REACT_APP_SHEET_ID=<replace with your sheet id> npm run build
```

4) copy the content of `build` folder to your server

### Recurring Expenses

Zapier is a service for connecting apps and automating your workflows. And it can be used to add recurring expenses with the [Google Sheets Integrations](https://zapier.com/zapbook/google-sheets/).

Select a trigger – it could be every month, week, or based on anything else.

Use the `Create Spreadsheet Row` integration and select your expense sheet and fill it with the desired values. Easy.

![Zapier setup for recurring expenses](doc/zapier.png)

### Sharing

Adding another person (for example your partner) to the app is easy – you just give them access to the expense sheet in Google Sheets.

After that, they have the same access as you are and can add expenses through the same URL.

---

