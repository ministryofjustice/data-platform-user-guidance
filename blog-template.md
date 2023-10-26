---
eleventyNavigation:
  key: [insert Blog title here in sentence case]
  parent: Blog
layout: post
title: [insert Blog title here in sentence case again]
date: [insert date here in format yyyy-mm-dd]
includeInBreadcrumbs: true
description: [insert date here without ordinal indicator, eg. 22 October 2023]
author: [insert author name here]
---

# Blog template

Use this template to write a blog post for the Data Platform front door (data-platform-user-guidance repository). Ensure the following:

* You create a copy of this template rather than edit the original
* You use Markdown syntax and save the file extension as .md
  * Note that the name of the file will show up in the URL
  * For best practice, name the file the same as the title but with hyphens, eg. my-blog-post.md
* You complete the front matter at the top of this file, removing the square brackets

Once you have written your blog post below, delete this entire section, including the heading and subheading, so that it does not appear in the published blog post.

You do not need to add a heading; the `title` setting in the front matter provides an h1 heading. Use h2 and h3 headings for subsections.

You also do not need to configure structuring. Just make sure you set the `date` correctly in the front matter, then drop the file in the docs>blog folder. Blog posts are configured to appear by most recent first.

## Publishing your blog post

If you are unfamiliar with the Git workflow, request help with publication from Jacob Woffenden or Soumaya Mauthoor. 

Or, if you are comfortable using the Git workflow, have assigned an SSH key to your GitHub account, and have installed Docker on your device:

1. Clone the data-platform-user-guidance repository using SSH:

`git clone git@github.com:ministryofjustice/data-platform-user-guidance.git`

2. Navigate to the root directory of the cloned repository on your device. If you have cloned it previously, first checkout the main branch:

`git checkout main`

and get the latest updates to the repository:

`git pull`

3. Create a branch to add your blog post file from:

`git checkout -b [new branch name]` 

4. Drag and drop your file into the docs>blog folder

5. Preview your changes:

`bash scripts/serve.sh`

6. If everything looks good, stage your changes:

`git add .`

then add a commit message:

`git commit -m "added a new blog post"`

7. Push the changes to the remote repository:

`git push origin [new branch name]`

8. Open a pull request on GitHub, assigning Jacob Woffenden as the reviewer.
