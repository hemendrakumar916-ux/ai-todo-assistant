# AI To-Do Assistant

A mobile-friendly GitHub Pages wrapper for a Google Apps Script To-Do web app.

## Backend URL

`https://script.google.com/macros/s/AKfycbzAdBR9_D86-02pFW7igbvbnfzdwjd7ineFeXwku06uvYPd9ZmNxJGPVS5RzcIKpcQY/exec`

## Features

- Add tasks from mobile
- Save tasks to Google Sheets
- Create Google Calendar events
- Receive mobile reminders
- Free static hosting with GitHub Pages

## Deploy

1. Create a public GitHub repository named `ai-todo-assistant`.
2. Upload `index.html`, `.nojekyll`, and `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Choose **Deploy from a branch**.
5. Select **main** and **/(root)**.
6. Click **Save**.
7. Wait about one minute for the live URL.

## Important

The frontend is hosted on GitHub Pages. Google Sheets and Calendar work through Google Apps Script.

The Apps Script `doGet()` should contain:

```javascript
.setXFrameOptionsMode(HtmlService.XFrameOptionsMode.ALLOWALL);
```
