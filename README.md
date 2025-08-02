# 🧪 Hands-On Lab: Running Tests with Nose

## 📂 Project Structure

```bash
labs/01_running_tests_with_nose/
├── my_code.py
├── test_my_code.py
├── setup.cfg
```

---

## ✅ Step-by-Step Lab Tasks

### ✅ Step 0: Set Up the Lab Environment

```bash
cd /home/project
git clone https://github.com/ibm-developer-skills-network/duwjx-tdd_bdd_PracticeCode.git
cd duwjx-tdd_bdd_PracticeCode/labs/01_running_tests_with_nose/
ls -l
```

---

### ✅ Step 1: Run Tests with Python `unittest`

Run all unit tests:

```bash
python3 -m unittest
```

Verbose output:

```bash
python3 -m unittest -v
```

---

### ✅ Step 2: Working with `nose`

Install Nose:

```bash
python3.8 -m pip install nose
```

Run with verbose:

```bash
nosetests -v
```

---

### ✅ Step 3: Add Color with `pinocchio`

Install `pinocchio`:

```bash
python3.8 -m pip install pinocchio
```

Run with spec and color:

```bash
nosetests --with-spec --spec-color
```

---

### ✅ Step 4: Add Test Coverage

Install `coverage`:

```bash
python3.8 -m pip install coverage
```

Run tests with coverage:

```bash
nosetests --with-spec --spec-color --with-coverage
```

---

### ✅ Step 5: Show Missing Coverage Report

```bash
coverage report -m
```

Optional: Generate an HTML report

```bash
coverage html
```

View in browser: `htmlcov/index.html`

---

### ✅ Step 6: Automate Nose Parameters with `setup.cfg`

Create `setup.cfg` in the same folder:

```ini
[nosetests]
verbosity=2
with-spec=1
spec-color=1
with-coverage=1
cover-erase=1
cover-package=triangle

[coverage:report]
show_missing = True
```

> 🔄 Replace `triangle` with your actual module name.

---

### ✅ Step 7: Run Tests Using Config

Now simply run:

```bash
nosetests
```

All configured parameters from `setup.cfg` will be applied.

---

## 🏁 Final Summary

Congratulations on completing the **Hands-On Lab: Running Tests with Nose**! 👏

You now know how to:

* Run unit tests using `unittest` and `nose`
* Enhance output with `pinocchio` for spec-style formatting and color
* Track code coverage using the `coverage` plugin
* Generate reports to identify untested code
* Automate test runs using a `setup.cfg` configuration file

These tools make your development process more **reliable**, **visual**, and **automated**. Now apply them in your own projects and CI/CD pipelines for robust Python testing!

---

Feel free to fork the lab repo and experiment further! 🧪💡

NAME - SOUVIK MANDAL
