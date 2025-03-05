# CODEOWNERS Demo

This repository demonstrates the use of the CODEOWNERS file in GitHub.

## About code owners

You can use a CODEOWNERS file to define individuals or teams that are responsible for code in a repository.

### CODEOWNERS file location

To use a CODEOWNERS file, create a new file called CODEOWNERS in the .github/, root, or docs/ directory of the repository, in the branch where you'd like to add the code owners. If CODEOWNERS files exist in more than one of those locations, GitHub will search for them in that order and use the first one it finds.

Each CODEOWNERS file assigns the code owners for a single branch in the repository. Thus, you can assign different code owners for different branches, such as @octo-org/codeowners-team for a code base on the default branch and @octocat for a GitHub Pages site on the gh-pages branch.

For code owners to receive review requests, the CODEOWNERS file must be on the base branch of the pull request. For example, if you assign @octocat as the code owner for .js files on the gh-pages branch of your repository, @octocat will receive review requests when a pull request with changes to .js files is opened between the head branch and gh-pages.

### More on code owners

Code owners are automatically requested for review when someone opens a pull request that modifies code that they own. Code owners are not automatically requested to review draft pull requests.

You can use a CODEOWNERS file to define individuals or teams that are responsible for code in a repository.

People with write permissions for the repository can create or edit the CODEOWNERS file and be listed as code owners. People with admin or owner permissions can require that pull requests have to be approved by code owners before they can be merged. This is done via branch protection.

The people you choose as code owners must have write permissions for the repository.

When the code owner is a team, that team must be visible and it must have write permissions, even if all the individual members of the team already have write permissions directly, through organization membership, or through another team membership.

If a file has a code owner, you can see who the code owner is before you open a pull request. In the repository, you can browse to the file and hover over to see a tool tip with codeownership details.

To use a CODEOWNERS file, create a new file called CODEOWNERS in the .github/, root, or docs/ directory of the repository, in the branch where you'd like to add the code owners.

If CODEOWNERS files exist in more than one of those locations, GitHub will search for them in that order and use the first one it finds.

Order is important; the last matching pattern takes the most precedence.

When reviews from code owners are required, an approval from any of the owners is sufficient to meet this requirement. For example, let's say that your CODEOWNERS file contains the following line:

*.js @global-owner1 @global-owner2

This means that changes to JavaScript files could be approved by either @global-owner1 or @global-owner2, but approvals from both are not required.
