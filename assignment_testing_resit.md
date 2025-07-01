# Assignment 1 - Testing - RESIT

The resit is individual, that is, not a group work.

## 1. Goal

The goal of this assignment is to experiment with test creation and coverage measurement. Each student will create their own project, develop test cases, measure test coverage, and refine or add new test cases to improve coverage.

## 2. Deliverables and Presentation

You must create a project and host it on a **private** GitHub repository. The URL of the repository must be submitted on Canvas, and access should be given to the TA assigned to evaluate your work (you will find this information in the presentation spreadsheet on the presentation day).

**The deliverables are**:

1. The repository URL: Submit it on Canvas.

2. Final report (`README.md`): Follow the template [here](assignment_testing_report_template_resit.md).

3. Presentation: Demonstrate the work and answer questions.

For the presentation, you should share your screen, and the evaluator will ask to go through the report. You must be prepared to execute parts of the code if requested.

**Deadlines**:

- Deadline for signing up for presentation (the link will come soon): 10th of July.

- Deadline for deliverables: 10th of July.

- Presentation day: 11th of July.

## 3. Tasks

### 3.0 Repository preparation

Your private GitHub repository should only contain a `README.md` file when created.

Then, you should create one application file (in either **Java or Python**). In the application file, you should create one function that:

- is structured in a way that allows it to be tested individually (with parameters and return values);

- contains at least one programming construct such as conditional and loop to ensure meaningful execution paths.

Having concluded this task, you can start to work on the following task.

### 3.1 Write an Initial Test Case

You must write **one test case** for the function at this point of the assignment. The test case:

- should validate expected behavior with assertions;

- be named following proper conventions (e.g., `{Function Name}_{Condition}_{Expected Result}`).

This task ensures that the project has some baseline tests before test coverage analysis begins.

### 3.2 Measure Initial Test Coverage

Now, it is time to measure how much of the function is actually covered by the initial test case. You should:

- use an existing coverage measurement tool (see suggestions in Section 5).

- analyze the results to identify which parts of the code are covered and which remain untested.

At this stage, your goal is to identify execution paths that remain untested and need further analysis.

### 3.3 Improve Coverage

Now that you have measured initial coverage, you will write additional test cases to ensure that more of the code of the function is tested.

You must write at least **one new test case** with inputs that force the program to take an uncovered path.

Once new test case is written, run the coverage tool again to check if test coverage has improved. Refine your test case (or write new ones) until the necessary coverage is achieved (which should be **the double of the coverage** found in Task 3.2).

### 3.4 Report (README.md)

At the end of the assignment, your work should be reported in the `README.md` file located at the root of your GitHub repository.
The `README.md` file should follow the assignment report template (see Section 2).

Note that the only considered files for evaluating the assignment should be in the main branch of the GitHub repository.

## 4. Evaluation and Grading

### 4.1 Eligibility

To have a grade > 0, the following criteria must be met:

* The work was done by a single person;

* The repository URL is submitted on Canvas by the deadline;

* There are no modifications in the repository after the deadline;

* The registration for a presentation slot is done by the deadline;

* The report (`README.md`) must exist in the main branch of the repository;

* You are present during the presentation (in case you cannot attend, a compelling reason should be provided to the teachers).

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
            <td>1) Creation of the initial test.</td>
            <td>
                <strong>1 Pt:</strong> There is evidence in the report that you created one initial test case.<br>
                <strong>0 Pts:</strong> Otherwise.
            </td>
            <td>1 pt</td>
        </tr>
        <tr>
            <td>2) Execution of existing coverage measurement tool on the initial test.</td>
            <td>
                <strong>1 Pt:</strong> There is evidence (screenshot of the results) that a tool was executed on the initial test.<br>
                <strong>0 Pts:</strong> Otherwise.
            </td>
            <td>1 pt</td>
        </tr>
        <tr>
            <td>3) Creation of new tests for coverage improvement.</td>
            <td>
                <strong>1 Pt:</strong> There is evidence (code) that you created at least one new test case.<br>
                <strong>0 Pts:</strong> Otherwise.
            </td>
            <td>1 pt</td>
        </tr>
        <tr>
            <td>4) Effectiveness of the new test(s) in improving coverage.</td>
            <td>
                <strong>1 Pt:</strong> There is evidence (screenshot of the old and new results) that the new test(s) improve coverage.<br>
                <strong>0 Pts:</strong> Otherwise.
            </td>
            <td>1 pt</td>
        </tr>
        <tr>
            <td>5) Organization and clarity of the report (`README.md`).</td>
            <td>
                <strong>1 Pt:</strong> The report follows the template and is clear.<br>
                <strong>0 Pts:</strong> The report is insufficient or does not follow the template.
            </td>
            <td>1 pt</td>
        </tr>
        <tr>
            <td><strong>Total</strong></td>
            <td></td>
            <td>5 pts</td>
        </tr>
    </tbody>
</table>

## 5. Suggestions

You can choose any coverage measurement tool for your project. The following are just examples:

* For Java: [Cobertura](https://cobertura.github.io/cobertura/), [JaCoCo](https://www.jacoco.org/jacoco/), and [OpenClover](https://openclover.org/).

* For Python: [Coverage.py](https://coverage.readthedocs.io/).
