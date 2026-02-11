# Wilcoxon Rank-Based Test Calculator

A lightweight browser-based calculator for:

- Wilcoxon Signed-Rank Test (Paired Samples)
- Mann–Whitney U Test (Wilcoxon Rank-Sum, Independent Samples)

This tool is designed for instructional use in statistics and data science courses.  
It runs entirely in the browser and requires no backend or installation.

---

## Features

- Choose Paired or Independent test
- Select alternative hypothesis (two-sided, greater, less)
- Accepts comma, space, or newline separated values
- Tie correction included
- Continuity correction included
- Works offline
- Canvas embeddable
- No external dependencies

---

## Statistical Methods

### Wilcoxon Signed-Rank Test (Paired)

- Removes zero differences
- Averages tied ranks
- Uses normal approximation with continuity correction

### Mann–Whitney U Test (Independent)

- Ranks combined samples
- Includes tie correction in variance
- Uses normal approximation with continuity correction

Note: For very small sample sizes, exact p-values may differ slightly from the normal approximation used here.

---

## How to Use

1. Select test type (Paired or Independent)
2. Choose alternative hypothesis
3. Enter numeric values in each box
4. Click Compute

The app returns:
- Test statistic
- z-score
- p-value

---

## Example Data

### Paired Example

X:
10 12 15 14 18

Y:
11 14 14 17 20

### Independent Example

Group 1:
5 7 8 9 6

Group 2:
10 12 9 11 8

---

## Canvas Embedding

Host the HTML file (wilcoxon_app.html) using:

- GitHub Pages
- Netlify
- University web server
- AWS S3

Then embed in Canvas using:

<iframe
  src="https://your-hosted-url.com/"
  width="100%"
  height="650"
  style="border:1px solid #ddd; border-radius:10px;"
></iframe>

---

## Technical Details

Language: HTML + JavaScript  
Backend: None  
Dependencies: None  
Distribution approximation: Normal  
Tie correction: Implemented  
Continuity correction: Implemented  

---

## Limitations

- Uses normal approximation (not exact distribution)
- No confidence intervals
- No effect size calculation
- No CSV upload

---

## License

MIT License
