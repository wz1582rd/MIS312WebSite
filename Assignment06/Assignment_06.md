# MIS312 Assignment 6 — Testing and Prompt Engineering

**Book Alignment:** Chapter 6  
**Primary Goal:** Practice a test mindset + improve AI prompts  
**Environment:** JupyterLab + VS Code (`.ipynb`)  
**Submission:** OneNote Artifact (PDF)

---

## Learning Objectives
- Write meaningful asserts
- Add one edge-case test
- Compare weak vs strong prompts

---

## Student Tasks

### Task 1 — Create a function
Create `assignment06_testing_prompts.ipynb`:
```python
def meal_total(base_price, tax_rate_percent, tip_rate_percent):
    """Return total meal cost including tax and tip."""
    tax = base_price * tax_rate_percent / 100
    tip = base_price * tip_rate_percent / 100
    return base_price + tax + tip
```

### Task 2 — Write asserts
```python
assert meal_total(50, 10, 15) == 62.5
assert meal_total(30, 5, 0) == 31.5
assert meal_total(100, 20, 25) == 145
```

### Task 3 — Add one edge-case assert
Example:
```python
assert meal_total(0, 10, 15) == 0
```

### Task 4 — Prompt comparison (required)
Compare:
- Weak: “Write a Python function for meal total.”
- Strong: includes exact function name/signature + asserts.

---

## VS Code Exercise — Turn This Into a Script (.py) and Troubleshoot

### Task 5 — Create a `.py` version in VS Code
1. Open **VS Code**.
2. Create a folder: `C:\Users\<StarID>\MIS312\assignment06\`
3. Create a file named: `meal_total.py`
4. Paste your function and asserts into the file (keep the asserts at the bottom).

Example structure:
```python
def meal_total(base_price, tax_rate_percent, tip_rate_percent):
    'Return total meal cost including tax and tip.'
    tax = base_price * tax_rate_percent / 100
    tip = base_price * tip_rate_percent / 100
    return base_price + tax + tip

# asserts (run as tests)
assert meal_total(50, 10, 15) == 62.5
assert meal_total(30, 5, 0) == 31.5
assert meal_total(100, 20, 25) == 145
assert meal_total(0, 10, 15) == 0

print("All asserts passed.")
```

### Task 6 — Run it from VS Code
- In VS Code, open **Terminal** → **New Terminal**
- Run:
```powershell
python meal_total.py
```

### Task 7 — Troubleshooting (required)
Deliberately cause one common beginner mistake, then fix it:
- Example: change one assert expected value to something incorrect, run, observe `AssertionError`, then fix it.
- Screenshot the error, then screenshot the successful run after your fix.

### Add to OneNote Artifact
- Screenshot of VS Code terminal showing success
- Screenshot of your deliberate error + fix
- Your `.py` code snippet (the function + asserts)


## OneNote Artifact Requirements
- Function + asserts
- Screenshot showing asserts ran successfully
- Weak vs strong prompt comparison
- Reflection: What makes a prompt strong?
