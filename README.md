# JEE Advanced Mock Test

A front-end clone of the JEE (Advanced) computer-based test interface, in one
HTML file. It adds one rule the practice portals don't have: the test runs in
fullscreen. Leave fullscreen once and you get a warning. Leave it a second time
and the paper is submitted automatically.

## Features

- **Login screen** that starts the test and enters fullscreen
- **48 questions** across Physics, Chemistry and Mathematics, with subject tabs
- **Four question types:** single correct, multiple correct, numerical answer and matching
- **Question palette** showing answered, not answered and not visited questions
- **3-hour countdown** that submits the paper when it reaches zero
- **Save & Next** and **Clear Response**, as in the real interface
- **Maths rendered with MathJax**
- **Results page** with the score per subject, correct and wrong counts, and a breakdown for every question

## Marking

| Type | Correct | Wrong |
| --- | --- | --- |
| Single correct, matching | +3 | −1 |
| Multiple correct | +4 (partial credit per correct option if none are wrong) | −2 |
| Numerical | +4 (within 0.2 of the answer) | 0 |

## Run

No build step. Open the file in a browser:

```bash
open jeeexam2.html
```

Log in with user ID `0000` and password `1111`.

## Stack

HTML, CSS and vanilla JavaScript. It uses the Fullscreen API, and MathJax
loaded from a CDN.
