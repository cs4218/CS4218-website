<frontmatter>
  title: "Milestone 2"
</frontmatter>

# Milestone 2

<div class="callout callout-warning">
  <div class="callout-title">Deadline</div>
  <p>Due on <strong>Week 10 Monday, 12:00 PM</strong>.</p>
</div>

## Integration Tests 👤

<div class="callout callout-info">
  <div class="callout-title">Weightage</div>
  <p>This section is worth <strong>2%</strong> of your final grade.</p>
</div>

- Design and write integration tests using the appropriate approaches, as discussed during the lectures.
- Integration tests are tests that test the interactions between different units. For example, it could be between a unit that you have tested previously during MS1 with another unit tested by another team member. Thus, you are no longer testing in isolation.
- Integration tests are white-box tests and hence will be written using the same technology and method as unit tests.
- Similar to Milestone 1:
  - Identify the integration tests to write and divide the workload equally among yourselves.
  - Note that the Suggested Testing Scope given is only for Milestone 1. As some components might have more interactions than others, feel free to re-allocate the components such that everyone has equal workload.
  - Also provide a clear indication of who did what:
    - Indicate each member's workload (i.e., who did what) in your repository's README file.
    - For every file you create or edit, include a comment at each location where you wrote test cases indicating your name and student ID (e.g., // John Doe, A0123456B).
    - This ensures that graders can clearly identify individual contributions and mark your work efficiently.
    - Failure to follow the above requirements will result in a 1 mark deduction.
  - There is no limit on the number of tests to write, write as many as you require.
  - You are required to fix any bugs found during testing.

### Grading Rubric

<div class="table-scroll course-note-table-scroll" role="region" aria-label="Project Milestone 2: 10% - Week 10 Monday 12 PM — Integration Tests 2% (Individual) — Grading Rubric" tabindex="0">
  <table class="wide-data course-note-table course-note-rubric">
    <thead>
      <tr>
        <th scope="col">Approach (0.5%)</th>
        <th scope="col">Correctness (1%)</th>
        <th scope="col">Variety (0.5%)</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>0: Integration tests were written without a clear approach or code does not match approach mentioned in the report.</td>
        <td>0.5: Integration tests are not testing integration of components or mocks/stubs are inappropriately used.</td>
        <td>0: Performed integration tests on less than 2 different component files.</td>
      </tr>
      <tr>
        <td>0.5: Integration tests are written with a clear approach (e.g., bottom-up integration, etc.) and the code aligns with the approach mentioned in the report.</td>
        <td>1: Integration tests are clearly testing the integration of some components, as opposed to complete mocking/stubbing in unit tests. This also means that mocks/stubs are appropriately used.</td>
        <td>0.5: Performed integration tests on at least 2 different component files (e.g. Login.js and Register.js instead of just varying levels of integration for Login.js).</td>
      </tr>
    </tbody>
  </table>
</div>

<div class="callout callout-success">
  <div class="callout-title">Submission</div>
  <p>Submit your code through tagging on GitHub. Tag your team's code as <strong>ms2</strong> in your GitHub repository.</p>
</div>

## UI Tests 👤

<div class="callout callout-info">
  <div class="callout-title">Weightage</div>
  <p>This section is worth <strong>3%</strong> of your final grade.</p>
</div>

- Identify end-to-end system tests. These are black-box tests and students need to use Playwright to develop these tests.
- These tests should test end-user scenarios that span across multiple components and tests, independent of the underlying implementation methods.
  - Good example of multiple components: User logs in -> adds item to cart -> views cart -> sees item in cart
  - Poor example of multiple components: Navigates to log in page -> checks that the page contains the necessary UI elements
- Similar to Milestone 1:
  - Identify the UI tests to write and divide the work equally among yourselves.
  - Note that the Suggested Testing Scope given is only for Milestone 1, re-allocate as necessary for equal workload.
  - Also provide a clear indication of who did what:
    - Indicate each member's workload (i.e., who did what) in your repository's README file.
    - For every file you create or edit, include a comment at each location where you wrote test cases indicating your name and student ID (e.g., // John Doe, A0123456B).
    - This ensures that graders can clearly identify individual contributions and mark your work efficiently.
    - Failure to follow the above requirements will result in a 1 mark deduction.
  - There is no limit on the number of tests to write, write as many as you require.
  - You are required to fix any bugs found during testing.

### Grading Rubric

<div class="table-scroll course-note-table-scroll" role="region" aria-label="Project Milestone 2: 10% - Week 10 Monday 12 PM — UI Tests 3% (Individual) — Grading Rubric" tabindex="0">
  <table class="wide-data course-note-table course-note-rubric">
    <thead>
      <tr>
        <th scope="col">Completeness (1%)</th>
        <th scope="col">Correctness (1%)</th>
        <th scope="col">Variety (1%)</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>0.5: Poor or incomplete E2E scenarios are tested. For example, just checking that a page has the necessary UI elements.</td>
        <td>0.5: UI tests are incorrectly implemented with poor structure (e.g., test case does not assert any outcomes).</td>
        <td>0.5: UI tests lack variety. For example, only implementing the test for 'Login successfully' and 'Login unsuccessfully'.</td>
      </tr>
      <tr>
        <td>1: Clear and complete E2E scenarios are tested. For example, for registration, the test case tests that the user navigates to register page, fill in details and finally register, instead of just checking that the register page has the necessary UI elements.</td>
        <td>1: UI tests are correctly implemented using Playwright with the structure of navigating to pages, performing user actions (e.g. clicking a button) and asserting the outcomes.</td>
        <td>1: UI tests are testing a variety of E2E user scenarios. For example, it is not sufficient to just implement 'Login successfully' and 'Login unsuccessfully'. Other diverse scenarios like 'Register' or 'View Profile' are included as well.</td>
      </tr>
    </tbody>
  </table>
</div>

<div class="callout callout-success">
  <div class="callout-title">Submission</div>
  <p>Submit your code through tagging on GitHub. Tag your team's code as <strong>ms2</strong> in your GitHub repository.</p>
</div>

## Code Coverage 👥

<div class="callout callout-info">
  <div class="callout-title">Weightage</div>
  <p>This section is worth <strong>1%</strong> of your final grade.</p>
</div>

- As a group, use SonarQube and generate a code coverage report.
- We are not grading based on how much code coverage has been obtained, but rather, we are grading based on the ability to run code coverage and generate these reports.
- Based on the generated report, write a **two-page summary**:
  - One page with screenshots of the report generated from SonarQube (e.g., percentages of different types of coverage, coverage for a specific file, etc).
  - Another page with your plan to improve the coverage based on the screenshots (you don't need to implement these proposed things).
  - If you have very high coverage (e.g., 99.5%), and thus, have very few things to write about in the second page, also describe your process of achieving high coverage. So you should write about:
    - The improvement plan for the small portion of code not yet covered (unless you attained 100%).
    - How your team attained high code coverage.

### Grading Rubric

<div class="table-scroll course-note-table-scroll" role="region" aria-label="Project Milestone 2: 10% - Week 10 Monday 12 PM — Code Coverage 1% (Group) — Grading Rubric" tabindex="0">
  <table class="wide-data course-note-table course-note-rubric">
    <thead>
      <tr>
        <th scope="col">Code Coverage Report (1%)</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>0: Did not use SonarQube OR insufficient details in sonarqube screenshots/improvement plan.</td>
      </tr>
      <tr>
        <td>1: Sufficient details for both SonarQube screenshots and improvement plan.</td>
      </tr>
    </tbody>
  </table>
</div>

<div class="callout callout-success">
  <div class="callout-title">Submission</div>
  <p>Submission on Canvas: Include this <strong>in your MS2 report submission.</strong></p>
</div>

## Report 👤

<div class="callout callout-info">
  <div class="callout-title">Weightage</div>
  <p>This section is worth <strong>4%</strong> of your final grade.</p>
</div>

- **Add 2 more pages** to your existing individual report with your approach for both Integration and UI tests (which approach you selected, why, etc.) and graphical test statistics for MS2 (things such as # of test identified, # tests automated, # of bugs identified, # of bugs fixed, etc.).
- **Add 1 more page** to include your group's progress for AI driven testing.
  - What have you done so far?
  - How effective was it?
  - Any improvements/changes you intend to make?
- **Add 2 more pages** to include your group's code coverage report.
- Feel free to update any details from MS1.
- Similar to Milestone 1:
  - Tables are **NOT** counted as graphical test statistics.
  - Effort marks will be awarded based on the quality and depth of the report content (compared against your peers).
  - The report has a **strict 2 page limit** for the individual component, a **strict 1 page limit** for the group AI-driven testing component, and a **strict 2 page limit** for the code coverage component.

### Grading Rubric

<div class="table-scroll course-note-table-scroll" role="region" aria-label="Project Milestone 2: 10% - Week 10 Monday 12 PM — Report 4% (Individual) — Grading Rubric" tabindex="0">
  <table class="wide-data course-note-table course-note-rubric">
    <thead>
      <tr>
        <th scope="col">Report (4%, this does not include code coverage)</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><strong>Two key components: approach description and graphical test statistics</strong></td>
      </tr>
      <tr>
        <td>1: Lacking in two key components (e.g., poor approach description and poor presentation of graphical test statistics).</td>
      </tr>
      <tr>
        <td>2: Lacking in only one key component.</td>
      </tr>
      <tr>
        <td>3: Good approach description and good presentation of graphical test statistics.</td>
      </tr>
      <tr>
        <td>+1/0: Additional marks based on effort (compared against peers).</td>
      </tr>
    </tbody>
  </table>
</div>

<div class="callout callout-success">
  <div class="callout-title">Submission</div>
  <p>Submission on Canvas:</p>
  <ul>
    <li>Collate the reports from your team members and submit one pdf file on Canvas (only one member needs to make the submission for the whole team).</li>
    <li>For example, a 5 member team should submit a 24 page pdf file on Canvas:
      <ul>
        <li>First 2 pages by member A (MS1)</li>
        <li>Next 2 pages by member A (MS2)</li>
        <li>Next 2 pages by member B (MS1)</li>
        <li>Next 2 pages by member B (MS2)</li>
        <li>…</li>
        <li>Page 21 and 22: Group's Code Coverage Report (MS2)</li>
        <li>Page 23: Group's plan for AI-driven testing (MS1, not graded but may be considered when determining effort marks)</li>
        <li>Page 24: Group's progress for AI-driven testing (MS2, not graded but may be considered when determining effort marks)</li>
      </ul>
    </li>
    <li>For the individual sections of the report, include a footer on every page stating your name and student ID (e.g., John Doe, A0123456B).</li>
    <li>Failure to follow the above mentioned requirements will result in a 1 mark deduction.</li>
    <li>A report cover page is optional and not necessary as long as it is clear who did what. Should you decide to include a cover page, it will <strong>NOT</strong> be counted towards the page limit.</li>
  </ul>
</div>
