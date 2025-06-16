# Assignment 2 - CI/CD

## 1. Goal

The goal of this assignment is to master the core of continuous integration and delivery. To achieve this goal, you are required to implement workflows with [GitHub Actions](https://docs.github.com/en/actions) on a repository.

Additionally, good collaboration practices within the team should be practiced.

## 2. Deliverables and Presentation

Each group must create a project and host it on a **private** GitHub repository. The URL of the repository must be submitted on Canvas, and access should be given to the TA assigned to evaluate your work (you will find this information in the presentation spreadsheet on the presentation day).

**The deliverables are**:

1. The repository URL: Submit it on Canvas.

2. Final report (`README.md`): Follow the template [here](assignment_cicd_report_template.md).

3. Presentation: Demonstrate the work and answer questions.

For the presentation, one group member should share their screen, and the evaluator will ask to go through the report and questions about the parts completed by each group member. The group must be prepared to execute parts of the code if requested.

**Deadlines**:

- Deadline for signing up for presentation (the link will come soon): 25th of June.

- Deadline for deliverables: 26th of June.

- Presentation day: 27th of June.

## 3. Tasks

### 3.0 Repository preparation

The private GitHub repository of your group should only contain a `README.md` file and a `LICENSE` when created. Then, the group should place their application and test code from Assignment 1 into the repository.

In case the group did not do Assignment 1, they should create one application file with at least one function and one test file with at least one test case that calls the application function.

Having concluded this task, your group can start to work on the following task.

### 3.1 Workflows with GitHub Actions

In total, each group must create 4 workflows in their repositories:

1. Testing (`testing.yml`): This workflow is dedicated to compiling and testing the project each time a commit is made on the repository. Compilation and testing should be done by calling a build tool.
2. Static analysis (`static_analysis_1.yml`): This workflow is dedicated to executing one static analysis tool to check for code quality attributes each time a commit is made on the repository.
3. Static analysis (`static_analysis_2.yml`): This workflow is also dedicated to executing one static analysis tool to check for code quality attributes. The only differences between this workflow and the previous one are that i) this should be only executed when a pull request is created in the repository and ii) a different static analysis tool should be used.
4. Release (`release.yml`): This workflow is dedicated to creating a release on GitHub each time a commit containing the word "release" in its message is made on the main branch of the repository.

At the end of this task, your repository should have the following structure:

```
your_project/
├── .github/
│   └── workflows/
│       ├── testing.yml
│       ├── static_analysis_1.yml
│       ├── static_analysis_2.yml
│       └── release.yml
├── src/
├── tests/
├── LICENSE
├── README.md
└── <other files, depending on the build tools your group is using>
```

### 3.2 Collaboration

Each group member must create one of the workflows mentioned above on their own individual git branches. Once a group member has the first complete version of a workflow, they should create a pull request using that git branch (amends on the workflow can be done later through other pull requests). Then, all the other group members should review it and leave comments in the pull requests if amends are necessary (this is because all group members should learn the workflows). Eventually, one reviewer merges the pull request into the main repository branch when everybody is fine with the workflow.

All pull requests should be merged by the deadline to avoid a resit.

### 3.3 Report (`README.md`)

The `README.md` file in the root of your repository should document your work following the provided template (see Section 2).

## 4. Evaluation and Grading

All group members will have the same grade. Individual participation is mandatory during the presentation.

### 4.1 Eligibility

To qualify for a grade, the following criteria must be met:

* The group is composed of more than one student;

* The repository URL is submitted on Canvas by the deadline;

* There are no modifications in the repository after the presentation;

* The registration for a presentation slot is done by the deadline;

* The report (`README.md`) must exist in the main branch of the repository and contain a statement of individual contributions;

* All group members are present during the presentation (in case a member cannot attend, a compelling reason should be provided to the teachers).

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
                <p><strong>4 Pts:</strong> There is evidence (link in the report and demonstration during the presentation) that the workflow works.</p>
                <p><strong>0 Pts:</strong> Otherwise.</p>
            </td>
            <td>4 pts</td>
        </tr>
        <tr>
            <td>3) Workflow #3.</td>
            <td>
                <p><strong>4 Pts:</strong> There is evidence (link in the report and demonstration during the presentation) that the workflow works.</p>
                <p><strong>0 Pts:</strong> Otherwise.</p>
            </td>
            <td>4 pts</td>
        </tr>
        <tr>
            <td>4) Workflow #4.</td>
            <td>
                <p><strong>4 Pts:</strong> There is evidence (link in the report and demonstration during the presentation) that the workflow works and that new automated releases contain a tag and files (code archive).</p>
                <p><strong>3 Pts:</strong> There is evidence (link in the report and demonstration during the presentation) that the workflow works and that new automated releases contain a tag but not files (code archive).</p>
                <p><strong>0 Pts:</strong> Otherwise.</p>
            </td>
            <td>4 pts</td>
        </tr>
        <tr>
            <td>5) Commit Messages.</td>
            <td>
                <p><strong>2 Pts:</strong> All or most commit messages are clear, follow a pattern, and are traceable.</p>
                <p><strong>1 Pts:</strong> Some commit messages follow the criteria.</p>
                <p><strong>0 Pts:</strong> Commit messages are unclear, messy, or follow different patterns.</p>
            </td>
            <td>2 pts</td>
        </tr>
        <tr>
            <td>6) Issue Tracking.</td>
            <td>
                <p><strong>2 Pts:</strong> Issues were consistently used to organize/track the group's work.</p>
                <p><strong>1 Pts:</strong> Some issues were used, but inconsistently.</p>
                <p><strong>0 Pts:</strong> No issues were created.</p>
            </td>
            <td>2 pts</td>
        </tr>
        <tr>
            <td>7) Pull Requests.</td>
            <td>
                <p><strong>2 Pts:</strong> Pull requests were consistently used and reviewed before merging.</p>
                <p><strong>1 Pts:</strong> Some pull requests were used, but inconsistently reviewed.</p>
                <p><strong>0 Pts:</strong> No pull requests were created.</p>
            </td>
            <td>2 pts</td>
        </tr>
        <tr>
            <td>8) Report (<code>README.md</code>).</td>
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
            <td>24pts</td>
        </tr>
    </tbody>
</table>

## 5. Ethics

This is teamwork. Therefore, be responsible and responsive to your teammates. Do not leave the tasks to be done at the last minute as this might cause stress for your teammates or impact the whole group's grade.

Moreover, information exchange and collaboration are fully allowed within your own groups. Cases of plagiarism or inter-group collaboration and assignment contents exchange will be reported to and managed by the official fraud committee. In case of fraud, the consequences of those acts may potentially lead to formal warning, inclusion of the formal warning in your VU student file, suspension from taking exams for a given period, expulsion from the VU.
