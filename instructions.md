# a0: Basic Tools  (1)
### Readings and Useful Documentation
* **Freeman & Ross (2019)** Refers to the course textbook, written by Mike Freeman and Joel Ross, *Programming Skills for Data Science: Start Writing Code to Wrangle, Analyze, and Visualize Data with R*, 2019. The book is available [online through the library](https://alliance-primo.hosted.exlibrisgroup.com/primo-explore/fulldisplay?docid=CP71294895890001451&context=L&vid=UW&lang=en_US&search_scope=all&adaptor=Local%20Search%20Engine&tab=default_tab&query=any,contains,programming%20skills%20for%20data%20science).
* **D'lgnazio & Klein (2020)** Refers to the course textbook, written by Catherine D'lgnazio and Lauren F. Klein, Data Feminism, 2020. The book is available [online at MIT Press](https://data-feminism.mitpress.mit.edu/)
* **Key documentation**: (1) [Markdown documentation on GitHub](https://guides.github.com/features/mastering-markdown/#GitHub-flavored-markdown); and (2) [The Emoji Cheat Sheet](https://github.com/ikatyang/emoji-cheat-sheet)

### Preparation
1. Please read: D'lgnazio & Klein (2020), the Introduction and chapter 1.
1. Please read: Freeman & Ross (2019), chapters 1-4.
1. Download and install [Atom](https://atom.io/).
2. Download and install [Git](https://git-scm.com/).
3. Sign-up for a [GitHub](https://github.com/) user account.
3. Configure git on your computer.
4. Download and install [R](https://cran.r-project.org/) (optional for this assignment but do it now).
5. Download and install [RStudio](https://www.rstudio.com/) (optional for this assignment but do it now).

<!--
### Notes on grading
* This assignment has **two parts** and is worth **34** points, as indicated in requirements below.
* Partial points can be awarded.
* All writing should be clear, concise, interesting, and free of spelling and grammatical errors.
* **Please note:** This assignment should be completed _individually_.
-->

### Notes on Professional Practice
1. **Get Started Early**. For any coding project, it is very important to get started earlier because unwelcome surprises often arise.
1. **Plan Your Work**. Before starting to design or code, read all of the requirements of this assignment, draw some sketches, and create a todo list of the steps you need to follow. It is almost always a good idea to do a bit of planning before starting to design or code.
1. **Communicate with Your TA**. If you find a requirement of this assignment _ambiguous_, you should ask your Teaching Assistant or post a question on Teams. The requirements of this assignment are intended to be clear and _unambiguous_, but, in general, this is very difficult to achieve. If something is unclear, always reach out to your teaching assistant (or  project manager or team member).

### Learning Objectives
1. Demonstrate how to navigate the file system from the command line and manage files, with these and similar commands (see F&R, chap. 2):
```
pwd             # print working directory
cd <PATH>       # change directory to <path>
cd ..           # change to parent directory (go up)
ls              # list files of current directory
ls -las         # list files (show some details)
#
mkdir <PATH>         # make a directory
rm <PATH>            # remove a file or directory
cp <PATH1> <PATH2>   # copy a file or directory
cat <FILENAME>       # display the contents of a file
```
2. Describe the purpose of git and GitHub (see Freeman & Ross, 2019, chap. 3).
3. Demonstrate how to manage a project using git and GitHub, with these and similar commands (see Freeman & Ross, 2019, chap. 3):
```
# Setting up basic identifying information
git config --global user.name <YOUR FULL NAME>
git config --global user.email <YOUR EMAIL ADDRESS>
#
git clone <REPO_URL>             # Copy a repo to your machine
git status                       # Check the status of a repo
git add <FILENAME>               # Add file to staging area
git add .                        # Add all files in current directory to  staging area
git git commit -m "<A MESSAGE>"  # Make changes s
git push
```
4. Use markdown syntax to format document (see Freeman & Ross, 2019, chap. 4).
5. Discuss _Data Feminism_ and explain how it provides a viewpoint for critically investigating data visualizations.

<!--
5. Consider how data science can be both a **tool** and a **weapon**.
6. Professional practice: (a) Work closely with requirements; and (b) Reflect on the benefits/costs of planning before doing.
-->



## Part I: The Command Line [10 points]
In Part I, you will practice working with the command line.

**Step #1**: In your directory, you will find a file named ``git-commands.md``. Open the file with Atom, which is our text editor.

**Step #2**: Following each prompt in the file ``git-commands.md``, write the line of code that you used to accomplish the task or otherwise answer the question.

**Step #3**: Save the changes to you've made to ``git-commands.md`` and then add, commit, and push your changes to GitHub.

**Note**: After completing this assignment, you can continue to add commands to this file and use it as a reference for your own work.

## Part II: Working with Markdown [35 points]

In Part II, you will create a report in Markdown.

### 1. Background
Please spend **ten minutes** or more scanning all the chapters in D'lgnazio & Klein (2020). You will find many different types of data visualizations. Some types will be quite familiar to you - see, for example, the bar charts in chapter 6. Others might be new or unusual, such as the iceberg in chapter 7.

### 2 Find Two Data Visualizations on the Internet
Browse the web and find two data visualizations that are **meaningful** to you. You might start, for example, at the [*New York Times*](http://nytimes.com) or [*Washington Post*](https://www.washingtonpost.com/) or other news source. That said, any scientific, cultural, government, or commercial institution website in the U.S. or beyond is just fine.

As you consider possible data visualizations, consider the following questions, which come from  D'lgnazio & Klein (2020, chap. 1):
1. **Who**: Who or what institution produced the visualization?
1. **Date**: When was it produced?
1. **Stakeholders**: Who is the audience for the visualization? And, who might be impacted, either directly or indirectly, by the visualization?
1. **Interests**: What values, goals, or interests are at stake with the visualization?
1. **Key facts**: What can be learned from the visualization?
1. **Power**: What issues, if any, are related to power are reflected in the data visualization?

**Note**: It may be difficult to answer these questions. That's okay; nevertheless, try as best as you can to formulate specific answers.

Once you have examined your two visualizations from a **Data Feminism** viewpoint, you need to select **one** of them as primary; the other visualization will be secondary. Now, you are ready to start coding (see next section).

### 3 Coding: Your Technical Requirements

Your objective is to create a report that presents your research and analysis. You will write your report using Markdown, which is a computer language for formatting text.

As you code with Markdown tags, please seek to create a professional visual appearance.

#### 3.1 Overall Requirements [3 points]
1. Include a title. [1 point]
1. Include your name. (you are the author of the report) [1 point]
1. Include the date of your report. [1 point]

#### 3.2 Filenames and Directory Requirements [5 points]
1. The name of the file containing your report should be ``README.md``. [1 point]
1. The ``README.md`` file containing your report should be located in the root directory of the repository. [1 point]
1. Create a new directory, named "a0-visualizations", within the "Images" directory. [1 point]
1. Put both your primary and secondary visualizations into this directory. [2 points]

#### 3.3 Your Report: What to include? [13 points]

First, your report should include a brief paragraph that summarizes what you did in your own words (about 100 words). In this paragraph you should name and link to both the **primary** and **secondary** data visualizations.  [5 points]

Second, for the primary data visualization, your report should include a description - that is, what specifically does the data visualization show? (about 100 words) [1 point]

Third, for the primary data visualization, write short responses after each of the headings, shown below. **Please note**: You should replace the `xxx (...)` with your own written response.

```
**Who**: xxx (20 words or less [1 point])
**Date**: xxx (a year (e.g, 2021) or more specific date about when the visualization was published [1 point])
**Stakeholders**: xxx (a short paragraph, 50 words or less [1 point])
**Interests**: xxx ([a short paragraph, 50 words or less [1 point])
**Key fact**: xxx (a short paragraph, 50 words or less [1 point])
```
Forth, and finally, conclude your report with a brief reflection (about 100 words), titled, "Data Feminism: What I Learned?" In this section, first, give a definition of data feminism from D'lgnazio & Klein (2020) and, second, briefly discuss what you learned by doing this assignment [2 points])

#### 3.4 Coding Requirements [14 points]
In your report you **MUST** use at each of these elements at least once:
  * A top-level heading (``Header1``) [1 point]
  * Three or more smaller headings (e.g., ``Header2``) [ 1 point]
  * An unordered list [1 point]
  * **Bold** for emphasis [1 point]
  * _Italics_ for emphasis [1 point]
  * Both ***Bold and Italics*** for emphasis [1 point]
  * An image tag to present the primary data visualization. Include the `ALT` tag and descriptive text for screen reader accessibility. (Note: See section 2.3 above) [2 points]
  * A blockquote to format the definition of "Data Feminism" [1 point]
  * Hypertext links to the websites that contain the primary and secondary data visualizations [2  points]
  * An emoji -- e.g., a rocket :rocket: -- in your reflective paragraph (Note: See emoji list: [cheat-sheet](https://github.com/ikatyang/emoji-cheat-sheet)) [1 point]
  * Include a footnote [2 points]

<!--
## Part III: Data Science: Tool for Good or Weapon?
A. Data science can be weapon, a tool that harms human beings. As we shall see, O'Neil (2016) presents a devastating critique of data science. We'll explore her arguments in some detail, but to start please answer these two questions from pages 1-14:
  1. By quoting from O'Neil (2016), define "Weapon of Math Destruction" (30-50 words). [1 point for accurate quote; 1 point for introducing and clarifying the quotation]
  2. Give an example of a WMD (30-50 words) [2 points for a complete example]

B. Data science can also, of course, be a tool for good. It can, for example, be used to make discovers about our social and natural worlds. One recent discovery made possible by data science is found in the paper by Wang, Stanovsky, Weihs, & Etzioni (2019). Browse this paper (see below for link) but please note: We do not expect you to understand the full paper in detail. Now, answer this question:
1. In your own words (a) what the the main research question; and (b) What did they find? (about 50 words) [1 point for (a); 1 point for (b)]

**Submission requirements.** Please create a file, named `data_science.md`, located the root directory of your repository. Write your answers with markdown in that file. Please format your answers neatly. Once you are finished, add, commit, and push all changes to GitHub.

Wang, L. L., Stanovsky, G., Weihs, L., & Etzioni, O. (2019). Gender trends in computer science authorship. CoRR, abs/1906.07883. Retrieved from http://arxiv.org/abs/1906.07883
-->
