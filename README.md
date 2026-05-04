# IT3040 Assignment 1 - Option 1

## Project Title
Automated Negative Testing for Chat-style Singlish to Sinhala Transliteration

## Objective
This project tests the Chat Sinhala transliteration function at:
https://www.pixelssuite.com/chat-translator

The test cases focus on incorrect transliteration results for informal Singlish input.

## Files Included
- `test_automation.py` - Playwright automation script
- `YOUR_REG_NUMBER_Test cases.xlsx` - Excel file containing 50 negative test cases
- `requirements.txt` - Python dependencies
- `Git_Repository_Link.txt` - Add your public GitHub repository link here
- `README.md` - Instructions to run the project

## Requirements
Install these before running:
- Python 3.11 or 3.12
- Google Chrome or Playwright Chromium

## Setup Steps
Open VS Code terminal inside this folder and run:

```bash
pip install -U pip
pip install -r requirements.txt
playwright install
```

## How to Run
Make sure the Excel file is closed before running the script.

```bash
python test_automation.py --excel "YOUR_REG_NUMBER_Test cases.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 5000 --type-delay-ms 80 --slow-mo-ms 200 --save-every 1 --keep-open
```

## Output
The script automatically writes results into the Excel file:
- Actual output
- Status

Status becomes:
- `PASS` when actual output exactly matches expected output
- `FAIL` when actual output differs from expected output

For this assignment, the final selected 50 test cases should be failing scenarios.
If any row becomes PASS, replace that test input with another failing case and rerun.

## Notes
- Do not keep Excel open while the script is running.
- Rename all files and the folder using your real registration number before submission.
- Push this folder to a public GitHub repository and paste the repository link in `Git_Repository_Link.txt`.
