# Assignment 1 - Testing

## 1. Goal

The goal of this assignment is to experiment with test creation and coverage measurement. Each group will create its own project, develop test cases, measure test coverage, and refine or add new test cases to improve coverage.

## 2. Deliverables and Presentation

Each group must create a project and host it on a **private** GitHub repository. The URL of the repository must be submitted on Canvas, and access should be given to the TA assigned to evaluate your work (you will find this information in the presentation spreadsheet on the presentation day).

**The deliverables are**:

1. The repository URL: Submit it on Canvas.

2. Final report (`README.md`): Follow the template [here](assignment_testing_report_template.md).

3. Presentation: Demonstrate the work and answer questions.

For the presentation, one group member should share their screen, and the evaluator will ask to go through the report and questions about the parts completed by each group member. The group must be prepared to execute parts of the code if requested.

**Deadlines**:

- Deadline for signing up for the presentation (the link for that will come soon): 11th of June.

- Deadline for deliverables: 12th of June.

- Presentation day: 13th of June.

## 3. Tasks

### 3.1 Define and Register Your Project

Each group will create a small, structured, and testable software project. The goal is to ensure that the project is simple enough to manage while being complex enough to make testing meaningful. The project can be written in **Java or Python** (that is, projects in other languages will not be accepted).

More details of the minimum criteria for the project and code structures to be used are available in Section 3.3 below.

Before starting, each group must define the purpose of their project and register it [here](https://docs.google.com/spreadsheets/d/1tYHh8h3cKHCUzhe6MnHL6ppBWpwk-FQYtmBd9rRg46E/edit?usp=sharing) (**do not request access to the file; be logged in with your VU email instead**). The description of the project proposal must be clear. Each group should check in the spreadsheet what the other groups have already registered because duplicate projects are not allowed.

### 3.2 Set Up Your GitHub Repository

Once your project is registered, the group will implement it collaboratively on a GitHub repository. The repository must include:

- A `src/` folder for all application source code;

- A `tests/` folder for all test code (test classes and test cases);

- A `README.md` file, which is the final report mentioned in Section 2.

### 3.3 Write Your Application Code Structured for Testability

The project must be modular to allow for test coverage analysis. Each group member must write **at least three functions** that perform distinct operations. Each function must:

- be structured in a way that allows it to be tested individually (with parameters and return values);

- contain at least one programming construct such as conditional and loop to ensure meaningful execution paths.

Once the project is fully implemented, the group will start testing it.

### 3.4 Write the Initial Test Cases

Each group member must write **one test case** for the project at this point of the assignment. The test case:

- can test any function of the project;

- should validate expected behavior with assertions;

- be named following proper conventions (e.g., `{Function Name}_{Condition}_{Expected Result}`).

The created tests must be placed in the `tests/` folder.

This task ensures that the project has some baseline tests before test coverage analysis begins.

### 3.5 Measure Initial Test Coverage

Now that each group member has written one test case, it is time to measure how much of the project is actually covered by these test cases.

- Use an existing coverage measurement tool (see suggestions in Section 5).

- Analyze the results to identify which parts of the code are covered and which remain untested.

At this stage, your goal is to identify functions or execution paths that remain untested and need further analysis.

### 3.6 Improve Coverage

Now that you have measured initial coverage, you will write additional test cases to ensure that more of the code is tested.

Each group member must write **two new test cases** with inputs that force the program to take those uncovered paths.

Once new test cases are written, run the coverage tool again to check if test coverage has improved. If some branches are still not covered, refine your test cases until the necessary coverage is achieved (which should be **the double of the coverage** found in Task 3.5).

### 3.7 Report (README.md)

At the end of the assignment, your group's work should be reported in the `README.md` file located at the root of your GitHub repository.
The `README.md` file should follow the assignment report template (see Section 2).

Note that the only considered files for evaluating the assignment should be in the main branch of the GitHub repository.

## 4. Evaluation and Grading

All group members will have the same grade. Individual participation is mandatory during the presentation.

### 4.1 Eligibility

To have a grade > 0, the following criteria must be met:

* The group is composed of more than one student;

* The chosen project is unique (that is, does not have the same purpose as another group's project);

* The repository URL is submitted on Canvas by the deadline;

* There are no modifications in the repository after the deadline;

* The registration for a presentation slot is done by the deadline;

* The report (`README.md`) must exist in the main branch of the repository and contain a statement of individual contributions;

* All group members are present during the presentation (in case a member cannot attend, a compelling reason should be provided to the teachers).

### 4.2 Grading Rubrics

<table data-full-width="true">
    <thead>
        <tr>
            <th width="242">Criteria</th>
            <th width="585">Ratings</th>
            <th>Points</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1) Creation of the project.</td>
            <td>
                <strong>2 Pts:</strong> There is evidence in the report that each member of the group implemented at least three functions of the application.<br>
                <strong>1 Pt:</strong> There is evidence in the report that members created functions, but not three per member.<br>
                <strong>0 Pts:</strong> Otherwise.
            </td>
            <td>2 pts</td>
        </tr>
        <tr>
            <td>2) Creation of the initial tests.</td>
            <td>
                <strong>2 Pts:</strong> There is evidence in the report that each member of the group created one test case.<br>
                <strong>1 Pt:</strong> There is evidence in the report that some members created one test case, but not all.<br>
                <strong>0 Pts:</strong> Otherwise.
            </td>
            <td>2 pts</td>
        </tr>
        <tr>
            <td>3) Execution of existing coverage measurement tool on the initial tests.</td>
            <td>
                <strong>2 Pts:</strong> There is evidence (screenshot of the results) that a tool was executed on the initial tests.<br>
                <strong>0 Pts:</strong> Otherwise.
            </td>
            <td>2 pts</td>
        </tr>
        <tr>
            <td>4) Creation of new tests for coverage improvement.</td>
            <td>
                <strong>2 Pts:</strong> There is evidence (code) that each student created two new test cases.<br>
                <strong>1 Pt:</strong> There is evidence (code) that the group created some new tests, but not two per member.<br>
                <strong>0 Pts:</strong> Otherwise.
            </td>
            <td>2 pts</td>
        </tr>
        <tr>
            <td>5) Effectiveness of each new test in improving coverage.</td>
            <td>
                <strong>2 Pts:</strong> There is evidence (screenshot of the old and new results) that the tests created by each member improve coverage.<br>
                <strong>1 Pt:</strong> There is evidence (screenshot of the old and new results) that some tests improve coverage, but not all.<br>
                <strong>0 Pts:</strong> Otherwise.
            </td>
            <td>2 pts</td>
        </tr>
        <tr>
            <td>6) Organization and clarity of the report (`README.md`).</td>
            <td>
                <strong>2 Pts:</strong> The report follows the template and is clear.<br>
                <strong>1 Pt:</strong> The report is sufficient for understanding but could be improved.<br>
                <strong>0 Pts:</strong> The report is insufficient or does not follow the template.
            </td>
            <td>2 pts</td>
        </tr>
        <tr>
            <td><strong>Total</strong></td>
            <td></td>
            <td>12pts</td>
        </tr>
    </tbody>
</table>

## 5. Suggestions

You can choose any coverage measurement tool for your project. The following are just examples:

* For Java: [Cobertura](https://cobertura.github.io/cobertura/), [JaCoCo](https://www.jacoco.org/jacoco/), and [OpenClover](https://openclover.org/).

* For Python: [Coverage.py](https://coverage.readthedocs.io/).

## 6. Ethics

This is teamwork. Therefore, be responsible and responsive to your teammates. Do not leave the tasks to be done at the last minute as this might cause stress for your teammates or impact the whole group's grade.

Moreover, information exchange and collaboration are fully allowed within your own groups. Cases of plagiarism or inter-group collaboration and assignment contents exchange will be reported to and managed by the official fraud committee. In case of fraud, the consequences of those acts may potentially lead to formal warning, inclusion of the formal warning in your VU student file, suspension from taking exams for a given period, expulsion from the VU.
