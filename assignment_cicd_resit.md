# Assignment 2 - CI/CD - RESIT

The resit is individual, that is, not a group work.

To resit, you must fill out a [form](https://docs.google.com/forms/d/e/1FAIpQLSeF1UxySFtoWq1fE2uSIJGoqWpc7nxB8f9B2f593IYDz59BmQ/viewform?usp=header) (you can access the spreadsheet with your VU email address) so that we can arrange the presentation day.

Deadline for registering: 6th of July (Sunday).

## 1. Goal

The goal of this assignment is to master the core of continuous integration and delivery. To achieve this goal, you are required to implement workflows with [GitHub Actions](https://docs.github.com/en/actions) on a repository.

## 2. Deliverables and Presentation

Each student must create a project and host it on a **private** GitHub repository. The URL of the repository must be submitted on Canvas, and access should be given to the TA assigned to evaluate your work (you will find this information in the presentation spreadsheet on the presentation day).

**The deliverables are**:

1. The repository URL: Submit it on Canvas.

2. Final report (`README.md`): Follow the template [here](assignment_cicd_report_template_resit.md).

3. Presentation: Demonstrate the work and answer questions.

For the presentation, you should share your screen, and the evaluator will ask to go through the report. You must be prepared to execute parts of the code if requested.

**Deadlines**:

- Deadline for signing up for presentation (the link will come soon): 10th of July.

- Deadline for deliverables: 10th of July.

- Presentation day: 11th of July.

## 3. Tasks

### 3.0 Repository preparation

Your private GitHub repository should only contain a `README.md` file and a `LICENSE` when created. Then, you should place your application and test code from Assignment 1 - RESIT into the repository.

In case you did not do Assignment 1 - RESIT, you should create one application file with at least one function and one test file with at least one test case that calls the application function (in either **Java or Python**).

Having concluded this task, you can start to work on the following task.

### 3.1 Workflows with GitHub Actions

In total, you must create 2 workflows in your repositories:

1. Testing (`testing.yml`): This workflow is dedicated to compiling and testing the project each time a commit is made on the repository. Compilation and testing should be done by calling a build tool.
2. Release (`release.yml`): This workflow is dedicated to creating a release on GitHub each time a commit containing the word "release" in its message is made on the main branch of the repository.

At the end of this task, your repository should have the following structure:

```
your_project/
├── .github/
│   └── workflows/
│       ├── testing.yml
│       └── release.yml
├── src/
├── tests/
├── LICENSE
├── README.md
└── <other files, depending on the build tools you are using>
```

### 3.2 Report (`README.md`)

The `README.md` file in the root of your repository should document your work following the provided template (see Section 2).

## 4. Evaluation and Grading

### 4.1 Eligibility

To qualify for a grade, the following criteria must be met:

* The work was done by a single person;

* The repository URL is submitted on Canvas by the deadline;

* There are no modifications in the repository after the presentation;

* The registration for a presentation slot is done by the deadline;

* The report (`README.md`) must exist in the main branch of the repository;

* You are present during the presentation (in case you cannot attend, a compelling reason should be provided to the teachers).

### 4.2 Grading Rubrics

<table>
    <thead>
        <tr>
            <th width="231">Criteria</th>
            <th width="443">Ratings</th>
            <th>Points</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1) Workflow #1.</td>
            <td>
                <p><strong>4 Pts:</strong> There is evidence (link in the report and demonstration during the presentation) that the workflow works.</p>
                <p><strong>0 Pts:</strong> Otherwise.</p>
            </td>
            <td>4 pts</td>
        </tr>
        <tr>
            <td>2) Workflow #2.</td>
            <td>
                <p><strong>4 Pts:</strong> There is evidence (link in the report and demonstration during the presentation) that the workflow works and that new automated releases contain a tag and files (code archive).</p>
                <p><strong>3 Pts:</strong> There is evidence (link in the report and demonstration during the presentation) that the workflow works and that new automated releases contain a tag but not files (code archive).</p>
                <p><strong>0 Pts:</strong> Otherwise.</p>
            </td>
            <td>4 pts</td>
        </tr>
        <tr>
            <td>3) Commit Messages.</td>
            <td>
                <p><strong>2 Pts:</strong> All or most commit messages are clear, follow a pattern, and are traceable.</p>
                <p><strong>1 Pts:</strong> Some commit messages follow the criteria.</p>
                <p><strong>0 Pts:</strong> Commit messages are unclear, messy, or follow different patterns.</p>
            </td>
            <td>2 pts</td>
        </tr>
        <tr>
            <td>4) Report (<code>README.md</code>).</td>
            <td>
                <p><strong>2 Pts:</strong> The report follows the template and is clear.</p>
                <p><strong>1 Pts:</strong> The report is sufficient for understanding but could be improved.</p>
                <p><strong>0 Pts:</strong> The report is insufficient or does not follow the template.</p>
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
