# Contributing to CyberArchive Blog

Thank you for your interest in contributing to the CyberArchive Blog! This blog is powered by [Hugo](https://gohugo.io/) and aims to provide a comprehensive index and archive of cybersecurity news and facts. Below is a guide to help you get started with contributing posts and factbytes.

## How to Contribute

If you are unfamiliar with GitHub or using Hugo, don’t worry! This guide will walk you through the process.

To learn about contributing with Github, please read the [Github documentation](https://docs.github.com/en/get-started/exploring-projects-on-github/contributing-to-a-project) first!

### Table of Contents

1. [Submitting a News Article](#submitting-a-news-article)
2. [Submitting a Factbyte](#submitting-a-factbyte)
3. [Folder Structure](#folder-structure)
4. [Guidelines](#guidelines)

## Submitting a News Article

1. **Create a new post file**:
   - Navigate to the following directory:  
     `<project-root>/cyberarchive/content/posts/`
   - Create a new markdown (`.md`) file. The file name must follow this format:
     ```
     YYYY-MM-DD-<article-name>.md
     ```
     For example, a post about an October 9th, 2024, article titled *Internet Archive Hacked* should be named:
     ```
     2024-10-09-internet-archive-hacked.md
     ```

2. **Article Template**:
   - Follow the template below to write your post:

     ```markdown
     ---
     title: <Title of the article>
     author: <Author's name>
     date: <Date of the article in ISO format (e.g., 2024-10-09T06:22:00+00:00)>
     draft: false
     categories:
       - <Category (e.g., data-breach, hacking)>
     tags:
       - <Relevant tags (e.g., industry_legal, phishing, ransomware)>
     ---

     [Original Article Link](<URL>)

     [Internet Archive Link](<Wayback Machine link if available>)

     ## Article Paste

     <Copy-paste relevant sections of the article. Add updates at the end if applicable.>
     ```

3. **Add relevant metadata**:
   - Ensure you add proper categories and tags for easy indexing.

4. **Submit via Pull Request**:
   - Once your post is complete, push it to your branch and open a Pull Request (PR) for review.

## Submitting a Factbyte

1. **Navigate to the factbytes directory**:
   - All cybersecurity facts are stored in the following folder:  
     `<project-root>/cyberarchive/content/pages/factbytes/`

2. **Add a fact under the appropriate year**:
   - Open the `factbytes.md` file and scroll to the section of the corresponding year.
   - Add a new fact in this format:
     ```markdown
     1. <Fact description> ([Source][source-link], <year>)
     ```

3. **Example Factbyte**:
   ```markdown
   ## Year 2023

   1. Cyberattacks on supply chains increased by 40% in 2023. ([Source][source-link], 2023)
   ```

4. **Update the source reference**:
   - Add a source link at the bottom of the file, like this:
     ```markdown
     [source-link]: https://example.com/source
     ```

5. **Submit via Pull Request**:
   - Once your factbyte is added, push your changes to your branch and open a Pull Request.

## Folder Structure

Here's an overview of the folder structure you'll be working with:

```
<project-root>
│
├── cyberarchive/
│   ├── content/
│   │   ├── posts/            # All news article posts go here
│   │   └── pages/
│   │       └── factbytes.md    # All factbytes are stored here
```

## Guidelines

- **Accuracy**: Please ensure that all facts and news posts are accurate and sourced from reputable publications.
- **Formatting**: Follow the templates provided for consistency.
- **References**: Always include links to original articles or studies.
- **Content Scope**: Content should focus on cybersecurity news, data breaches, cybercrime trends, and relevant security facts/statistics.

By following these guidelines, you help keep the CyberArchive organized and useful to its audience.

Thank you for contributing!