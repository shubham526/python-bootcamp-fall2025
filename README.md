# Python Bootcamp for Industry Professionals

[![University](https://img.shields.io/badge/University-UMSL-blue.svg)](https://www.umsl.edu/)
[![Python](https://img.shields.io/badge/Python-3.8+-green.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

A comprehensive 2-day intensive Python bootcamp designed for working professionals with no prior programming experience. Learn practical automation, data analysis, and visualization skills through hands-on projects.

**Instructor:** Dr. Shubham Chatterjee  
**Institution:** University of Missouri–St. Louis  
**Contact:** shubham.chatterjee@mst.edu

---

## 📚 Course Overview

This bootcamp transforms complete beginners into confident Python practitioners through:
- **16 contact hours** of intensive, hands-on training
- **80% practical coding** with real-world business problems
- **7 comprehensive notebooks** covering fundamentals to data science
- **6 guided projects** you can adapt for your own work

### What You'll Learn
- Python fundamentals (variables, data types, control flow)
- Data structures (lists, dictionaries, sets)
- Functions and object-oriented programming
- File I/O and error handling
- Data analysis with pandas
- Data visualization with matplotlib

---

## 🗂️ Repository Structure

```
python-bootcamp-fall2025/
├── Day1/
│   ├── Chap1_Variables_Strings_Numbers.ipynb
│   ├── Chap2_Lists_Loops_Conditionals_Dicts.ipynb
│   ├── Chap3_Functions_Classes.ipynb
│   ├── Chap4_Files_Exceptions.ipynb
│   └── projects/
│       ├── project_server_log_analyzer.ipynb
│       ├── project_expense_processor.ipynb
│       └── project_email_cleaner.ipynb
├── Day2/
│   ├── Chap5_Pandas.ipynb
│   ├── Chap6_Matplotlib.ipynb
│   └── projects/
│       ├── project_api_dashboard.ipynb
│       ├── project_finance_tracker.ipynb
│       └── project_fitness_analyzer.ipynb
└── README.md
```

---

## 🚀 Getting Started

### Option 1: Google Colab (Recommended)
No installation required! Click the "Open in Colab" buttons below to run notebooks directly in your browser.

### Option 2: Local Installation

If you prefer to run notebooks locally, we recommend using **Conda** as it handles Python installation and package management seamlessly.

#### Recommended: Using Conda (Easiest for Beginners)

**What is Conda?**
Conda is an all-in-one package and environment manager that comes with Anaconda or Miniconda. It includes Python and makes installing data science packages much simpler.

**Anaconda vs Miniconda:**
- **Anaconda:** Full distribution (~3GB) with 250+ pre-installed packages. Good if you have disk space and want everything ready.
- **Miniconda:** Minimal installer (~400MB) with just Python and conda. You install only what you need. **We recommend this.**

**Step 1: Install Miniconda**
1. Download Miniconda from [docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html)
2. Run the installer and follow the prompts
3. **Important:** Check "Add Miniconda to PATH" during installation (or restart your terminal after installation)

**Step 2: Clone the Repository**
```bash
git clone https://github.com/YOUR-USERNAME/python-bootcamp-umsl.git
cd python-bootcamp-umsl
```

**Step 3: Create Conda Environment**
```bash
# Create environment named 'bootcamp' with Python 3.10 and all required packages
conda create -n bootcamp python=3.10 pandas matplotlib seaborn numpy jupyter requests -y

# Activate the environment
conda activate bootcamp
```

After activation, you'll see `(bootcamp)` at the start of your command prompt.

**Step 4: Launch Jupyter Notebook**
```bash
jupyter notebook
```

This opens Jupyter in your browser. Navigate to the notebook you want to work with.

**Step 5: When You're Done**
```bash
# Deactivate the environment
conda deactivate
```

**For Future Sessions:**
```bash
# Just activate and launch
conda activate bootcamp
jupyter notebook
```

---

#### Alternative: Using pip and venv (If You Already Have Python)

If you already have Python 3.8+ installed, you can use virtual environments with pip.

**What is a Virtual Environment?**
A virtual environment is an isolated Python workspace that keeps project dependencies separate. It prevents package conflicts between different projects.

**Setup Steps:**

**On macOS/Linux:**
```bash
# Clone repository
git clone https://github.com/YOUR-USERNAME/python-bootcamp-umsl.git
cd python-bootcamp-umsl

# Create virtual environment
python3 -m venv venv

# Activate it
source venv/bin/activate

# Install packages
pip install --upgrade pip
pip install pandas matplotlib seaborn numpy jupyter requests

# Launch Jupyter
jupyter notebook

# When done
deactivate
```

**On Windows:**
```bash
# Clone repository
git clone https://github.com/YOUR-USERNAME/python-bootcamp-umsl.git
cd python-bootcamp-umsl

# Create virtual environment
python -m venv venv

# Activate it
venv\Scripts\activate

# Install packages
pip install --upgrade pip
pip install pandas matplotlib seaborn numpy jupyter requests

# Launch Jupyter
jupyter notebook

# When done
deactivate
```

---

#### Troubleshooting

**"conda: command not found"**
- Restart your terminal after installing Miniconda
- Or manually add Conda to PATH: Run the Miniconda installer again and ensure "Add to PATH" is checked

**"python3: command not found" (for venv method)**
- You need to install Python first from [python.org](https://www.python.org/downloads/)
- Or switch to the Conda method above

**Jupyter won't start**
```bash
# Make sure your environment is activated first
conda activate bootcamp  # or: source venv/bin/activate

# Then try launching again
jupyter notebook
```

**Can't see notebooks in Jupyter**
- Make sure you're in the `python-bootcamp-umsl` directory when you run `jupyter notebook`
- Navigate using Jupyter's file browser

**Windows Execution Policy Error (venv method)**
```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

---

#### Quick Command Reference

**Conda:**
```bash
conda activate bootcamp      # Start working
jupyter notebook            # Launch Jupyter
conda deactivate            # Stop working

conda env list              # See all environments
conda list                  # See installed packages
```

**Venv:**
```bash
source venv/bin/activate    # Start (Mac/Linux)
venv\Scripts\activate       # Start (Windows)
jupyter notebook            # Launch Jupyter
deactivate                  # Stop
```

---

## 📖 Day 1: Python Fundamentals & Automation

### Chapter 1: Variables, Strings, Numbers & Input
Learn Python basics including variables, data types, string manipulation, user input, and f-strings.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shubham526/python-bootcamp-fall2025/blob/main/Day1/Chap1.ipynb)

**Topics Covered:**
- Variables and assignment
- Strings and string methods
- Numbers (integers and floats)
- User input with `input()`
- F-strings for formatting
- Comments and code documentation

---

### Chapter 2: Lists, Loops, Conditionals & Dictionaries
Master essential data structures and control flow for organizing and processing data.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shubham526/python-bootcamp-fall2025/blob/main/Day1/Chap2.ipynb)

**Topics Covered:**
- Lists: creation, indexing, slicing, methods
- For loops and while loops
- Conditional statements (if/elif/else)
- Dictionaries: key-value pairs
- Looping through dictionaries
- List comprehensions

---

### Chapter 3: Functions & Classes
Write reusable, modular code using functions and object-oriented programming.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shubham526/python-bootcamp-fall2025/blob/main/Day1/Chap3.ipynb)

**Topics Covered:**
- Defining and calling functions
- Parameters and return values
- Default arguments and keyword arguments
- Creating classes with `__init__`
- Instance attributes and methods
- Inheritance basics

**Practice Projects:**
- BankAccount class
- Bank management system

---

### Chapter 4: Files & Exceptions
Handle file operations and errors gracefully to build robust applications.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shubham526/python-bootcamp-fall2025/blob/main/Day1/Chap4.ipynb)

**Topics Covered:**
- Reading and writing text files
- The `with` statement
- Exception handling with try-except
- Working with JSON data
- File paths and error handling

**Practice Projects:**
- To-do list manager
- Interactive file-based application

---

### Day 1 Mini-Projects

#### Project A: Server Log Analyzer
Build a tool to parse server logs, identify patterns, and generate reports.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shubham526/python-bootcamp-fall2025/blob/main/Day1/projects/project_server_log_analyzer.ipynb)

**Skills Applied:** File I/O, string parsing, dictionaries, functions, error handling

---

#### Project B: Expense Report Processor
Create an automated expense categorization and reporting system.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shubham526/python-bootcamp-fall2025/blob/main/Day1/projects/project_expense_processor.ipynb)

**Skills Applied:** CSV parsing, dictionaries, aggregations, error handling, formatting

---

#### Project C: Email List Cleaner
Develop a contact list validator and deduplication tool.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shubham526/python-bootcamp-fall2025/blob/main/Day1/projects/project_email_cleaner.ipynb)

**Skills Applied:** String validation, sets, file operations, data cleaning

---

## 📊 Day 2: Data Analysis & Visualization

### Chapter 5: Data Analysis with Pandas
Master the essential library for data manipulation and analysis.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shubham526/python-bootcamp-fall2025/blob/main/Day2/Chap5.ipynb)

**Topics Covered:**
- Series and DataFrame objects
- Reading CSV files
- Data selection with loc and iloc
- Filtering and boolean indexing
- Handling missing data
- GroupBy operations
- Aggregations and pivot tables

**Real Dataset:** Sales data analysis with revenue, regions, and products

---

### Chapter 6: Data Visualization with Matplotlib
Create professional, publication-ready visualizations.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shubham526/python-bootcamp-fall2025/blob/main/Day2/Chap6.ipynb)

**Topics Covered:**
- Figure and Axes architecture
- Line plots, scatter plots, histograms
- Customizing colors, styles, and markers
- Adding labels, titles, and legends
- Subplots for multiple visualizations
- Professional styling

**Real Dataset:** Movie budget and revenue analysis

---

### Day 2 Capstone Projects

#### Option A: Public API Dashboard
Build a command-line dashboard that fetches and displays live API data.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shubham526/python-bootcamp-fall2025/blob/main/Day2/projects/project_api_dashboard.ipynb)

**Skills Applied:** API requests, JSON parsing, data processing, error handling

---

#### Option B: Personal Finance Tracker
Create an interactive expense tracking application with persistent storage.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shubham526/python-bootcamp-fall2025/blob/main/Day2/projects/project_finance_tracker.ipynb)

**Skills Applied:** Classes, JSON storage, user input, data aggregation

---

#### Option C: Fitness/Workout Analyzer
Analyze workout logs and visualize training progress over time.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shubham526/python-bootcamp-fall2025/blob/main/Day2/projects/project_fitness_analyzer.ipynb)

**Skills Applied:** Pandas data analysis, matplotlib visualization, data cleaning

---

## 🔗 Additional Resources

### Quick Reference Guides
- [Python Cheat Sheet](https://www.pythoncheatsheet.org/)
- [Python Quick Reference](https://quickref.me/python)

### Pandas Resources
- [Official Pandas Cheat Sheet (PDF)](https://pandas.pydata.org/Pandas_Cheat_Sheet.pdf)
- [DataCamp Pandas Guide](https://www.datacamp.com/cheat-sheet/pandas-cheat-sheet-for-data-science-in-python)

### Matplotlib Resources
- [Official Matplotlib Cheat Sheets](https://matplotlib.org/cheatsheets/)
- [DataCamp Matplotlib Guide](https://www.datacamp.com/cheat-sheet/matplotlib-cheat-sheet-plotting-in-python)

### Further Learning
- [Python Official Documentation](https://docs.python.org/3/)
- [Real Python Tutorials](https://realpython.com/)
- [Kaggle Learn](https://www.kaggle.com/learn)
- [DataCamp](https://www.datacamp.com/)

---

## 💡 How to Use This Repository

### For Bootcamp Participants
1. **Before the bootcamp:** Familiarize yourself with Google Colab by clicking any "Open in Colab" button
2. **During the bootcamp:** Follow along with the instructor using the Colab notebooks
3. **After the bootcamp:** Use the notebooks as reference materials and adapt the projects for your work

### For Self-Learners
1. Work through Day 1 notebooks sequentially (Chapters 1-4)
2. Complete at least one Day 1 mini-project
3. Progress to Day 2 notebooks (Chapters 5-6)
4. Challenge yourself with a Day 2 capstone project
5. Modify projects to work with your own data

### Tips for Success
- **Code along** - Don't just read, type the code yourself
- **Experiment** - Modify examples to see what happens
- **Debug** - Errors are learning opportunities
- **Practice** - Complete the exercises in each notebook
- **Build** - Adapt projects to solve your real-world problems

---

## 🤝 Contributing

Found a typo or bug? Have a suggestion for improvement? Contributions are welcome!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -am 'Add new example'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a Pull Request

---

## 📧 Contact & Support

**Instructor:** Dr. Shubham Chatterjee  
**Email:** shubham.chatterjee@mst.edu  
**LinkedIn:** [linkedin.com/in/shubham-chatterjee](https://www.linkedin.com/in/shubham-chatterjee)

For bootcamp enrollment, questions, or corporate training inquiries, please reach out via email.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- University of Missouri–St. Louis for hosting this bootcamp
- All bootcamp participants for their enthusiasm and feedback
- The Python community for excellent open-source tools and documentation

---

## 🎓 Certificate of Completion

Bootcamp participants who complete both days and submit projects will receive an official certificate from the University of Missouri–St. Louis documenting 16 contact hours of Python training.

---

**Ready to start your Python journey? Click any "Open in Colab" button above and begin coding!**
