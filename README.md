# Introduction to Git and Collaborative Development

### Workshop Overview

In this workshop, participants will learn the basics of Git and collaborative web development on GitHub. They will:

1.  Clone a repository.
2.  Create a new branch for a new feature.
3.  Make changes to an HTML file.
4.  Push the branch to the remote repository.
5.  Create a pull request.
6.  Merge the branch into the main branch.
7.  Collaboratively modify the HTML file.
8.  Resolve merge conflicts.

### Prerequisites

-   Participants should have Git installed on their computers.
-   Access to GitHub accounts.

### Workshop Materials

-   A sample HTML repository on GitHub.
-   Initial HTML file (index.html) with simple content.
-   Workshop guide (step-by-step instructions).

#### Initial HTML File (index.html)

```html
<!DOCTYPE html>
<html>
<head>
    <title>My Website</title>
</head>
<body>
    <h1>Welcome to My Website</h1>
    <p>This is the initial content.</p>
</body>
</html>
```

### Workshop Steps

**Step 1: Clone the Repository**

-   Each participant should open their terminal or Git GUI tool.
-   Navigate to the directory where they want to clone the repository.
-   Use the following command to clone the repository (replace `<repository_url>` with the URL of your sample repository on GitHub):


    ```bash
    git clone <repository_url>
    ```

**Step 2: Create a New Branch**

-   Inside the cloned repository directory, create a new branch for your feature:

    ```bash
    git checkout -b feature-A1-branch
    ```

**Step 3: Make Changes to the HTML File**

-   Open the `index.html` file in a text editor.
-   Modify the file by adding a new paragraph, e.g.:

    ```html
    <p>This is the new feature added by Programmer A</p>
    ```

**Step 4: Commit Changes**

-   Save your changes in the text editor.
-   In the terminal, commit your changes:

    ```bash
    git add index.html
    git commit -m "Add new feature to index.html by Programmer A"
    ```

**Step 5: Push the Branch to GitHub**

-   Push the branch to the remote repository on GitHub:

    ```bash
    git push origin feature-A1-branch
    ```

**Step 6: Create a Pull Request on GitHub**

-   Go to your GitHub repository.
-   You will see a prompt to create a pull request. Click on it.
-   Select the base branch (e.g., `main`) and the feature branch (`feature-A1-branch`).
-   Add a title and description for your pull request.
-   Create the pull request.

**Step 7: Merge the Branch**

-   Review the pull request with your partner or workshop facilitator.
-   Merge the branch into the main branch on GitHub.

**Step 8: Collaboratively Modify the HTML File**

-   Now, both programmers will continue to work on the same `index.html` file.
-   Make different changes to the HTML file (e.g., add new paragraphs, headings, or images) independently.

**Step 9: Create Conflict by editing the same lines**

-   Programmer A edits the <h1> heading of index.html file:

```html
<h1>Welcome to My HTML Website</h1>
```

-   Programmer B edits the same line in index.html:

```html
<h1>Welcome to My Amazing Website</h1>
```

**Step 10: Attempt to merge and experience a conflict**

-   Both programmers attempt to merge their changes into the main branch on GitHub.
-   Conflicts occur due to simultaneous edits.

**Step 11: Resolve merge conflicts**

-   Collaboratively resolve conflicts by discussing and editing the conflicting parts of `index.html`.

    Programmer A's changes:

    ```html
    <h1>Welcome to My HTML Website</h1>
    ```

    Programmer B's changes:

   ```html
   <h1>Welcome to My Amazing Website</h1>
   ```


-   Decide on the final content, and make sure it makes sense. For example, you can combine both changes to preserve both contributions:

    Resolved content:

    ```html
   <h1>Welcome to My Amazing HTML Website</h1>
   ```

-   Save the changes in the text editor.

**Step 12: Commit and Merge the Resolved Changes**

-   In the terminal, commit the resolved changes:

    ```bash
    git add index.html
    git commit -m "Resolve merge conflict between Programmer A and Programmer B"
    ```

-   Push the changes to the remote repository:

    ```bash
    git push origin feature-B-branch
    ```

-   Go to your GitHub repository.
-   Review the pull request that had the conflict.
-   Confirm that the conflicts are resolved and the final content is as expected.
-   Now, to merge the resolved branch (feature-branch) into the main branch, use the following Git commands:

    ```bash
    # Switch to the main branch
    git checkout main
    
    # Merge the feature branch into the main branch
    git merge feature-B-branch
    ```
-   If the merge is successful and there are no further conflicts, you can push the changes to GitHub:

    ```bash
    git push origin main
    ```

### Workshop Tips for Conflict Resolution
-   Discuss best practices for resolving merge conflicts.
-   Emphasize the importance of clear commit messages and descriptive pull request descriptions.
-   When resolving conflicts, it's essential to ensure that the resulting code is correct and coherent. In the example above, we combined both changes by both programmers into a single coherent sentence.
-   Always thoroughly test the resolved code to make sure it functions as intended.
-   Encourage participants to communicate effectively during conflict resolution to ensure everyone understands the changes made and the reasons behind the final resolution.
-   You can also demonstrate different conflict resolution strategies, such as choosing one version over another or manually editing to create a new version.

#### Workshop Conclusion

Participants have successfully learned how to resolve merge conflicts in Git and GitHub collaboratively, ensuring that their collaborative code is coherent and functional. This skill is valuable in real-world team projects where multiple contributors are working on the same codebase. Provide further resources for participants to continue learning about Git and GitHub best practices.
