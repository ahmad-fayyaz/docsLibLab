## Adding Documentation to the Docs Website

Welcome to the LibLab's documentation website's guide! Follow the steps below to add new documentation to our website, edit existing documentation or remove documentation.

### Prerequisites

-   Access to the GitHub repository of the website.
-   Knowledge of Markdown syntax.
-   Knoweldge of accessibility practices used in writing documentation.

### Steps to Add New Documentation

1.  **Clone the Repository**
    
First, clone the repository to your local machine if you haven't already:

```
git clone https://github.com/your-username/your-repo.git
```

```
cd your-repo
```    

2. **Open the folder in Visual Studio Code** or code editor of your choice.
3. **Create a New Markdown File**

Inside the  `docs`  directory in `src`, create a new Markdown file for your documentation. Each file is stored accordingly into a folder. Make sure to follow existing categorisation rules. For example, to add a new guide for ArtSteps, create a file named  `new-guide.md` in the ArtSteps folder.

4. **Write Your Content**

Open the newly created file in your preferred text editor and add your content using Markdown syntax. Here’s an example:

```markdown
# New Guide

## Introduction

This is the introduction to the new guide.

## Section 1

Detailed information about the first section.

## Conclusion

Final thoughts and summary.
```

To learn more about markdown, [click this link.](https://www.markdownguide.org)

5. **Update Sidebar Configuration**

To make your new guide accessible via the sidebar, update the sidebar configuration in the  `docs/.vitepress/config.mts`file. You will see all the headings neatly organized. Simply add:

```
{  text:  'New Guide',  link:  '/path/to/the/file'  }
```

under the heading you want it to be. 


6. **Commit and Push Changes**

After making your changes, commit and push them to the repository:

```
git add .
```
```
git commit -m "Add new guide to documentation" 
```
```
git push origin main
```

7. **Deploy the Changes**

The website should be set up to deploy automatically upon push.

8. **Done**


Enjoy the day, you did it! Wasn't that hard, right?
