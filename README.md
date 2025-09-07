# [Assignment Type]: [Assignment Title]
## 🎯 Overview & Purpose
<!--
INSTRUCTOR NOTE:
Write a brief, high-level paragraph explaining the purpose of this assignment.
What is the core problem the student is trying to solve?
Why is it important in the context of the course?
-->
In this assignment, you will practice [Core Concept] by building a [Brief Description of Program]. This will reinforce your understanding of [Skill 1] and [Skill 2].
## 📚 Learning Objectives
Upon successful completion of this assignment, you will be able to:
<!--
INSTRUCTOR NOTE:
List 2-4 specific, measurable learning objectives for this assignment.
-->
- [Objective 1, e.g., "Implement functions that use pointers to modify variables."]
- [Objective 2, e.g., "Decompose a problem into smaller, testable functions."]
- [Objective 3, e.g., "Follow a professional, feature-branch Git workflow."]
## 📋 Instructions & Requirements
<!--
INSTRUCTOR NOTE:
This is the core of the assignment. Provide the detailed prompt, scenario,
and a clear, numbered list of all functional requirements.
-->
### The Scenario
[Provide a clear and engaging scenario for the assignment.]
### Core Requirements
You must implement the following functionality:
1. **Requirement 1:** [Detailed description of the first requirement.]
2. **Requirement 2:** [Detailed description of the second requirement.]
3. **Requirement 3:** [And so on...]
### Constraints
- You must adhere to the C++ Core Guidelines for naming and style.
- [Add any other constraints, e.g., "No global variables allowed," "Must use a struct to represent X," etc.]
## ⚙️ Workflow & Submission
Follow these steps carefully to set up your environment and submit your work.
### Part 1: Initial Setup
1. **Accept the Assignment:** Use the GitHub Classroom link on Canvas to create your assignment repository.
2. **Clone the Repository:** In your Home Codespace, clone your new assignment repository.
3. **Add to Workspace:** In the VS Code file explorer, right-click in the empty space below your Home folder and select "Add Folder to Workspace...". Choose your assignment folder to add it.
### Part 2: Development Cycle
1. **Create a Branch:** Before writing any code, create a new branch for your work. Use our standard naming conventions (`add/`, `fix/`, `update/`).
```bash
git checkout -b add/feature-name
```
2. **Write Your Code:** Implement the required features in the appropriate `src/` and `include/` files.
3. **Run the Tests:** The `tests/` directory contains a suite of automated tests to help you verify your code. **You should not modify these files.** To run the tests, follow these steps in your terminal:
```bash
    # 1. Configure CMake (only needs to be done once)
    cmake -S . -B build

    # 2. Build the project (including your code and the tests)
    cmake --build build

    # 3. Run the tests
    cd build
    ctest --output-on-failure
    cd .. 
```
  Your goal is to get all tests to pass.
  
4. **Commit Your Changes:** Commit your work in small, logical chunks. Remember to use `git add <file>` to stage only the specific files you changed and write a clear, semantic commit message.
```bash
    git add src/my_file.cpp include/my_file.h
    git commit -m "feat: implement the core calculation logic"
```
### Part 3: Submission
1. **Push Your Branch:** Once your code is complete and all tests are passing, push your branch to GitHub.
```bash
    git push origin add/feature-name
```
