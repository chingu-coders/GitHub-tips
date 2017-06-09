# GitHub Tips by Chingu

[Contributing guidelines](CONTRIBUTING.md)


## Table of Contents

- [Purpose](#the-purpose-of-this-repo)
- [About Chingu](#the-chingu-github-organization)
- [Collaborating on GitHub](#collaborating-on-github---a-tale-of-two-models)
- [GitHub Organizations](#working-with-organizations)

## The Purpose of this Repo

GitHub.com is an amazing code collaboration platform which has enabled several open source project to flourish. Contributing to projects on GitHub for those new to the platform, however, can be both intimidating and confusing. This repo aims to provide some clarity on the features and workflows of GitHub.

## The Chingu GitHub Organization

[Chingu](https://tropicalchancer.github.io/projectus/) is a self-organizing coding bootcamp community and innovative collaboration project. It's also now a GitHub organization! The reasons for this organization's existence include the following:

1. Provide Chingu members with a safe place to practice and participate in code collaboration workflows
2. Deliver visibility to all Chingu members on what their peers are working on and have accomplished
3. Curate a refined selection of resources to support Chingu members in achieving their learning and career goals

## Collaborating on GitHub - A Tale of Two Models

There are two predominate models for collaborating on GitHub projects:

 * **[Fork & Pull Model](https://en.wikipedia.org/wiki/Fork_and_pull_model)**: This is the predominate model used by open-source projects on GitHub. The project has a core group of project maintainers but many more potential contributors. The high-level workflow involves:

    1. Contributor [forks](https://help.github.com/articles/fork-a-repo/) the main project repo to their user account
    1. Contributor creates a [branch](https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell) and completes their work locally (more on this later)
    1. Contributor [pushes](https://help.github.com/articles/pushing-to-a-remote/) to their user account and submits a [pull request](https://help.github.com/articles/about-pull-requests/) (PR)
    1. Project maintainer is notified of PR and one or more of several things can happen next - discussion on the PR, continuous integration (CI) tests, acceptance of the PR (with or without edits), rejection of the PR

 * **Shared Repository Model**: In this model, everyone works on the same repo and there is no forking. The advantage is decreased complexity with the drawback of less control. This model is ideal for projects where the expected contributors are already known - for example - the Chingu build.to.learn projects! The high-level workflow involves:

    1. Contributor creates a branch and completes their work locally (details to come)
    1. Contributor pushed branch to shared repo
    1. Contributor creates a pull request (PR) into master from their branch, optionally [assigning a reviewer](https://help.github.com/articles/assigning-issues-and-pull-requests-to-other-github-users/)
    1. Reviewer is notified of PR and one or more of several things can happen next - discussion on the PR, continuous integration (CI) tests, acceptance of the PR (with or without edits), rejection of the PR

For both models, [different rules](https://help.github.com/articles/enabling-required-status-checks/) can be created as to what is required before acceptance of a PR and corresponding merge of changes into the master branch. In any case, directly pushing to master from local is either not allowed or just not good practice as it prevents the opportunity for conservation and code review on the desired changes.

Both of these workflows follow what is called "GitHub flow" illustrated here in this [GitHub guide](https://guides.github.com/introduction/flow/).

## Working with Organizations

Note: Much of this is distilled from the [information provided here](https://help.github.com/categories/setting-up-and-managing-organizations-and-teams/)

### Organization and Roles

We have started with an organization for all the Chingu coders. All members who requested access were added with the **Member** role. With the **Member** role, you can:

1. Create repos
1. Create teams and be made a team maintainer
1. See all members and teams
1. Create or delete project boards and edit descriptions

There is also the **Owner** role who can invite and delete members, add billing information and delete the organization. This role will be provided on request to cohort leads and others with the need and to apply these features.

### Teams and Organization Repos

#### Organization Repos 

As mentioned previously all team members have the ability to create organization repos. They then have the ability to change permissions on that [repo for different users](https://help.github.com/articles/repository-permission-levels-for-an-organization/#changing-repository-settings]) so that specific people can collaborate.

To better organize permissions on a repo there are **Teams**.

#### Teams

Any organization member can create a team which is the perfect equivalent to the Chingu build.to.learn teams. To do so, click on the **Teams** tab then click **New**.

*TODO*: Suggest naming convention for teams and repos.

After creation, you will be taken to the team page. Here you can add members by clicking the **Add a member** button then search by username, full name, or email. Click on the user to add them. You will be prompted for your password before continuing.

If they are in the organization they will automatically added. If they are not, then an invite will be sent to them which they must accept. For more [see the docs](https://help.github.com/articles/adding-organization-members-to-a-team/).

After adding, team members can be promoted to the **Maintainer** role. Maintainers have the [following permissions](https://help.github.com/articles/repository-permission-levels-for-an-organization/#team-maintainers). 

#### Team Repos

Those with admin access to an organization repo (the creator, those granted admin access, or the organization owner) can add that repo to any team they belong to. To do so, click on the **Repositories** tab, click **Add repository** then search for the repo and select it.

Now all members of the team will have Admin access. This access can be changed by navigating to **Settings** then **Collaborators & team** within the repo. More about repository permission levels can be [read here](https://help.github.com/articles/repository-permission-levels-for-an-organization/).

*TODO*:

* [ ] Diagrams? Maybe with (draw.io)[https://www.draw.io/]
* [ ] Technical details on how to follow GitHub Flow with examples