# MIS312 Assignment 5 — Reading Python Code: Part 2

**Book Alignment:** Chapter 5  
**Primary Goal:** Understand branching logic and function behavior on different inputs  
**Environment:** JupyterLab (`.ipynb`)  
**Submission:** OneNote Artifact (PDF)

---

## Learning Objectives
- Explain `if/elif/else`
- Predict outcomes for multiple inputs
- Explain why functions return different results

---

## Student Tasks

### Task 1 — Conditionals (predict output)
Create `assignment05_reading2.ipynb` and paste:
```python
temperature = 72
if temperature > 80:
    print("Hot")
elif temperature >= 60:
    print("Comfortable")
else:
    print("Cold")
```

Predict then run. Change temperature to **55** and **85**; run and record output.

### Task 2 — Read a function and explain it
Paste:
```python
def grade_letter(score):
    if score >= 90:
        return "A"
    elif score >= 80:
        return "B"
    elif score >= 70:
        return "C"
    elif score >= 60:
        return "D"
    else:
        return "F"

print(grade_letter(88))
print(grade_letter(59))
```

Explain why those results occur.

### Task 3 — AI review (required)
Ask:
> “What are two common mistakes beginners make with if/elif/else code?”

Write the suggestions and how you will avoid them.

---

## OneNote Artifact Requirements
- Outputs for all temperatures (screenshots)
- Function snippet + your explanations
- AI prompt + summary
- Reflection: Which part of conditionals is still confusing?
