<a href="https://waffle.io" target='_blank'><img src="https://img.shields.io/badge/waffle.io-dependency-yellowgreen.svg" /></a>

# Scrum Base Repository

This is for when you want to start an public github project and you want to manage your scrum workflow for free, without depending on project management tools that you'll eventually need to pay for. Pull requests and issue templates are already setup for you, however to copy in labels follow instructions in the installation section.

# HOWTO : Use GitHub for scrum workflow

##### Credit goes to https://github.com/jvandemo/github-scrum-workflow/blob/master/README.md

<img src="https://cloud.githubusercontent.com/assets/1859381/5397698/9972fe22-815c-11e4-8be6-21e1d0d05849.jpg" alt="codecat" align="right">

Turn any public GitHub repository into a simple but powerful agile work environment.

**Summary:**
+ [Installation Instructions](#install-instructions) 
+ [How it works](#how-it-works)
+ [1. Create issues as backlog items](#1-create-issues-as-backlog-items)
+ [2. Add labels to issues](#2-add-labels-to-issues)
+ [3. Define sprints as milestones](#3-define-sprints-as-milestones)
+ [Overview](#overview)
+ [Helpful links](#helpful-links)
+ [Change log](#change-log)

---

## How it works

- Backlog items are reported as **issues**
- Meta data are assigned to items as **labels** or in the case of **points** you should you waffle.io.
- **milestones** are used to group issues in sprints


## Installation Instructions

```sh
git clone git@github.com:CSProjectsEAL/ScrumBaseRepository.git
```

- Go into the newly created folder and run the following command:

```sh
 rm -r remove .git
```

- Initialise the git and push the base to a new repository.

```sh
	git init
	git remote add origin [NameOfRepository]
	git push -u origin master
```

### Copy labels from this repository
	- Open the github.com/yourusername/newreponame/labels page
	- Open the js developer console in your browser. 
	- Copy in the script found in the gist below:

- https://gist.github.com/alex855k/69de4efdc7464eb904cbd3ea3df61dfa

- Add this infront

```sh
	git init
	git remote add origin [NameOfRepository]
	git push -u origin master
```

## 1. Create issues as backlog items

To create a new backlog item, just create a new issue.

Once a new issue has been created, assign it the right labels and/or assign it to a sprint (milestone).

Issues allow you to have a conversation about the item and even allow you to create task lists inside the issue using [GitHub's markdown](https://guides.github.com/features/mastering-markdown/).

## 2. Add labels to issues

Add the following labels to your repository:

### Priorities

When assigning

`priority` labels allow you to prioritize items in your backlog e.g.:

- `priority: low` Could implement this.
- `priority: medium` Should implement this.
- `priority: high` Must implement this.

### Points

Points meta-data is added using the wrapping project management framework waffle.io.

Waffle.io allows you to assign velocity points to individual items (issues) e.g. using [Fibonacci numbers](http://en.wikipedia.org/wiki/Fibonacci_number).

Based on these you can generate graphs based velocity etc. in waffle.io

To use waffle.io just add the repository through the /CSEALProjects organisation.

### Types

`type` labels allow you to easily filter items (issues) in the dashboard e.g.:

- `type:bug`: bug
- `type:hotfix`: fix that requires immediate attention
- `type:feature`: a suggestion for a new feature
- `type:story`: a new feature in the shape of description from the point of view of a user note: stories should be written so they are <a href="https://agileforall.com/vertical-slices-and-scale/" target="_blank">vertically sliced</a>
- `type:infrastructure`: infrastructure related change or addition
- `type:performance`: performance related issue
- `type:refactor`: Contribution issue: related to refactoring, if something is missing abstraction or not adhering to coding standards
- `type:test`: Contribution issue: for review test related issues, if something is missing from the tests, acceptance criteria etc.

### Other

You can define and assign custom labels that you need within your workflow or organization.

## 3. Define sprints as milestones

You can create a milestone for every sprint and add items (issues) from the backlog to a milestone.

This allows you to group items in sprints and track them by milestone in your [issue dashboard](https://github.com/issues).

The backlog then consists of all items (issues) that have no `milestone` attached to it.

**TIP**: Use `no:milestone` in the search field on your [issue dashboard](https://github.com/issues) to find backlog items.

## Overview

![en_overview](https://cloud.githubusercontent.com/assets/1859381/5411950/c44c229e-8207-11e4-915f-d31ccd66c5bd.png)

Image: [Scrum primer](http://www.scrumprimer.org/overview).

## Helpful links

- [Mastering GitHub issues](https://guides.github.com/features/issues/)
- [Mastering GitHub markdown](https://guides.github.com/features/mastering-markdown/)
- [GitHub Flavored Markdown](https://help.github.com/articles/github-flavored-markdown/)
- [How to write pull requests](https://help.github.com/articles/github-flavored-markdown/)