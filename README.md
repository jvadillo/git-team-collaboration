# Introduction to Git and Collaborative Development

#### Workshop Overview

In this workshop, participants will learn the basics of Git and collaborative web development on GitHub. They will:

1.  Clone a repository.
2.  Create a new branch for a new feature.
3.  Make changes to an HTML file.
4.  Push the branch to the remote repository.
5.  Create a pull request.
6.  Merge the branch into the main branch.
7.  Collaboratively modify the HTML file.
8.  Resolve merge conflicts.

#### Prerequisites

-   Participants should have Git installed on their computers.
-   Access to GitHub accounts.

#### Workshop Materials

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

#### Workshop Steps

Step 1: Clone the Repository

-   Each participant should open their terminal or Git GUI tool.
-   Navigate to the directory where they want to clone the repository.
-   Use the following command to clone the repository (replace `<repository_url>` with the URL of your sample repository on GitHub):


    ```bash
    git clone <repository_url>
    ```

Step 2: Create a New Branch

-   Inside the cloned repository directory, create a new branch for your feature:

    ```bash
    git checkout -b feature-branch
    ```

Step 3: Make Changes to the HTML File

-   Open the `index.html` file in a text editor.
-   Modify the file by adding a new paragraph, e.g.:

    ```html
    <p>This is the new feature added by <Your Name></p>
    ```

Step 4: Commit Changes

-   Save your changes in the text editor.
-   In the terminal, commit your changes:

    ```bash
    git add index.html
    git commit -m "Add new feature to index.html"
    ```

Step 5: Push the Branch to GitHub

-   Push the branch to the remote repository on GitHub:

    ```bash
    git push origin feature-branch
    ```

Step 6: Create a Pull Request on GitHub

-   Go to your GitHub repository.
-   You will see a prompt to create a pull request. Click on it.
-   Select the base branch (e.g., `main`) and the feature branch (`feature-branch`).
-   Add a title and description for your pull request.
-   Create the pull request.

Step 7: Merge the Branch

-   Review the pull request with your partner or workshop facilitator.
-   Merge the branch into the main branch on GitHub.

Step 8: Collaboratively Modify the HTML File

-   Now, both programmers will continue to work on the same `index.html` file.
-   Make different changes to the HTML file (e.g., add new paragraphs, headings, or images) independently.

Step 9: Resolve Merge Conflicts

-   Attempt to merge the changes into the main branch on GitHub.
-   Conflicts will likely occur due to simultaneous edits.
-   Collaboratively resolve conflicts by discussing and editing the conflicting parts of `index.html`.
-   Commit the resolved changes.
-   Merge the branch into the main branch.

#### Workshop Tips

-   Encourage participants to collaborate closely during conflict resolution.
-   Discuss best practices for resolving merge conflicts.
-   Emphasize the importance of clear commit messages and descriptive pull request descriptions.
-   Encourage participants to experiment with branching, making more changes, and resolving conflicts.

#### Workshop Conclusion

Participants have learned the basics of Git, collaborative development, and conflict resolution on GitHub. They can now apply these skills to real-world team projects and contribute effectively to collaborative coding efforts. Provide resources for further Git and GitHub learning, such as documentation and tutorials.
