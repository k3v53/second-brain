---
title: 
aliases: 
tags:
  - English
  - GitHub
  - Discussions
draft: false
status: Backlog
---
> [!todo]

GitHub Discussions uses YAML to describe a template and uses the [GitHub Form Schema](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/syntax-for-githubs-form-schema).

## [Creating discussion category forms](https://docs.github.com/en/discussions/managing-discussions-for-your-community/creating-discussion-category-forms#creating-discussion-category-forms)

People with write access to a repository can create a discussion category form.

1. Navigate to the repository where you want to create a discussion category form.
2. In your repository, create a file called `/.github/DISCUSSION_TEMPLATE/FORM-NAME.yml`, replacing `FORM-NAME` with the name for your discussion category form. The name must correspond with the slug for one of your discussion categories. For example, the template for the "Announcements" category should be `.github/DISCUSSION_TEMPLATE/announcements.yml`. For more information about creating new files on GitHub, see "[Creating new files](https://docs.github.com/en/repositories/working-with-files/managing-files/creating-new-files)."
3. In the body of the new file, type the contents of your discussion category form. For more information, see "[Syntax for discussion category forms](https://docs.github.com/en/discussions/managing-discussions-for-your-community/syntax-for-discussion-category-forms)."
4. Commit your file to the default branch of your repository. For more information, see "[Creating new files](https://docs.github.com/en/repositories/working-with-files/managing-files/creating-new-files)."
# Sources
- https://github.com/orgs/community/discussions/2838
	- https://docs.github.com/en/discussions/managing-discussions-for-your-community/syntax-for-discussion-category-forms
		- https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/syntax-for-githubs-form-schema
	- https://github.blog/2023-01-09-github-discussions-just-got-better-with-category-forms/