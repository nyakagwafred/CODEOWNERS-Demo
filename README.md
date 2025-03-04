# CODEOWNERS Demo
This repository demonstrates the use of the CODEOWNERS file in GitHub.

## About code owners
You can use a CODEOWNERS file to define individuals or teams that are responsible for code in a repository.

### CODEOWNERS file location
To use a CODEOWNERS file, create a new file called CODEOWNERS in the .github/, root, or docs/ directory of the repository, in the branch where you'd like to add the code owners. If CODEOWNERS files exist in more than one of those locations, GitHub will search for them in that order and use the first one it finds.

Each CODEOWNERS file assigns the code owners for a single branch in the repository. Thus, you can assign different code owners for different branches, such as @octo-org/codeowners-team for a code base on the default branch and @octocat for a GitHub Pages site on the gh-pages branch.

For code owners to receive review requests, the CODEOWNERS file must be on the base branch of the pull request. For example, if you assign @octocat as the code owner for .js files on the gh-pages branch of your repository, @octocat will receive review requests when a pull request with changes to .js files is opened between the head branch and gh-pages.
