# Contributing to CyberArchive Blog (Docusaurus Edition)

Thank you for your interest in contributing to the CyberArchive Blog! This site is powered by [Docusaurus](https://docusaurus.io/) and aims to provide a comprehensive index and archive of cybersecurity news and facts. Below is a guide to help you get started with contributing posts and statistics.

## How to Contribute

If you are unfamiliar with GitHub or using Docusaurus, don’t worry! This guide will walk you through the process.

To learn about contributing with GitHub, please read the [GitHub documentation](https://docs.github.com/en/get-started/exploring-projects-on-github/contributing-to-a-project) first!

### Table of Contents

1. [Submitting a News Article](#submitting-a-news-article)  
2. [Submitting a Factbyte](#submitting-a-factbyte)  
3. [Folder Structure](#folder-structure)  
4. [Guidelines](#guidelines)

---

## Submitting a News Article

1. **Create a new post file**:  
   - In a standard Docusaurus setup, blog posts reside in the `blog/` folder (e.g., `<project-root>/blog/`).  
   - Create a new Markdown (`.md` or `.mdx`) file in the `blog/` folder.  
   - The file name should follow this format for clarity:  
     ```
     YYYY-MM-DD-<article-name>.md
     ```
     For example, a post about an October 9, 2024, article titled *Internet Archive Hacked* should be named:
     ```
     2024-10-09-internet-archive-hacked.md
     ```

2. **Article Template**:  
   - At the top of your Markdown file, include Docusaurus front matter. Below is a sample template:

     ```markdown
     ---
     title: <Title of the article>
     slug: <unique-slug-for-the-article> 
     authors: [<Author's name>]
     date: 2024-10-09
     tags: [<relevant-tags>]
     ---

     [Original Article Link](<URL>)

     [Internet Archive Link](<Wayback Machine link if available>)

     ## Article Paste

     <Copy-paste relevant sections of the article. Add updates at the end if applicable.>
     ```

   - Adjust the keys (such as `title`, `slug`, `authors`, `date`, and `tags`) as necessary. Docusaurus automatically sorts blog posts by date.

3. **Add relevant metadata**:  
   - Ensure you add proper tags for easy indexing.  
   - If you need multiple authors, you can use the array format in `authors`.

4. **Submit via Pull Request**:  
   - Once your post is complete, commit the file, push it to your branch, and open a Pull Request (PR) for review.

---

## Submitting a Factbyte

1. **Navigate to the statistics location**:  
   - We maintain cybersecurity “statistics” in a dedicated documentation file. For example:  
     ```
     <project-root>/docs/statistics/statistics.md
     ```
     (Adjust this path if your project uses a different structure.)

2. **Add a fact under the appropriate year**:  
   - Open the relevant `statistics.md` file and locate the section for the current year (or create one if it doesn’t exist).
   - Add a new fact using a format like:

     ```markdown
     ## Year 2024

     1. Cyberattacks on supply chains increased by 40% in 2023. ([Source][source-link], 2023)
     ```

     Make sure you increment the numbering accordingly and update the text/year as needed.

3. **Update the source reference**:  
   - At the bottom of the `statistics.md` file, add or update the source link reference:

     ```markdown
     [source-link]: https://example.com/source
     ```

4. **Submit via Pull Request**:  
   - Once your factbyte is added, commit the changes, push them to your branch, and open a Pull Request.

---

## Folder Structure

Here’s an example overview of the folder structure for this Docusaurus project (your structure may vary):

```
<project-root>
│
├── blog/
│   └── 2024-10-09-internet-archive-hacked.md   # Example blog post
│
├── docs/
│   └── statistics/
│       └── statistics.md                       # All statistics are stored here
│
├── docusaurus.config.js
├── package.json
└── ...
```

---

## Guidelines

- **Accuracy**: Ensure that all facts and news posts are accurate and sourced from reputable publications.  
- **Formatting**: Follow the templates provided for consistency.  
- **References**: Always include links to original articles, studies, or reputable sources.  
- **Content Scope**: Focus on cybersecurity news, data breaches, cybercrime trends, and relevant security facts/statistics.  

By following these guidelines, you help keep the CyberArchive organized and useful to its audience.

Thank you for contributing!