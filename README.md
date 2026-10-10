
# Tansik Egypt

A free web tool for Egyptian students on the **American Diploma, IGCSE and IB DP** tracks. It calculates your high-school GPA, then estimates your **Egyptian Tansik total** from your GPA and your SAT / EST / ACT scores, and lists the government faculties that total qualifies for.

**Live site:** https://tansik-egy.gpa-egy.workers.dev/

## Features

- **GPA calculator** for American Diploma, IGCSE (letters A*–U and numbers 9–1) and IB DP.
- **Tansik estimator** that takes your GPA out of 4 and your test scores (SAT, EST, ACT) and gives the total, with separate rules for government and private universities.
- **ACT to EST conversion** for the Math and English sections.
- **Faculties table** (Arabic, right-to-left) showing the government faculties whose minimum is at or below your total, with search.
- Buttons to the official Tansik limits page and the government application page.
- **Save as PDF** of your result.
- Responsive, white and blue theme, no sign-up, no data leaves your browser.

## How the total is estimated

- GPA part: `GPA / 4 × 40`
- First test: `total / 1600 × weight`, where the weight is 60, or 69 (government) / 75 (private) when the total is at least 1090.
- Second test: `total / 1600 × 15`, counted only when the two-subject sum reaches 1100 (government) / 900 (private).
- Minimum first-test total: 1050 (government) / 800 (private).

## Important notes

- This is an **estimate**. The official result comes only from the Egyptian coordination office.
- The faculty minimums come from a table I compiled; always check the official limits page before applying.
- The tool is independent and is not affiliated with any government body.

## Tech

Plain HTML, CSS and JavaScript in a single static page. Hosted on Cloudflare Workers static assets.

## Author

Made by **Abdulrahman Abed**. © 2026 Abdulrahman Abed. All rights reserved.
