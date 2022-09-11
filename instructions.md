# A1: Basic Tools  (1)
### Readings and Useful Documentation
* **Freeman & Ross (2019)** Refers to the course textbook, written by Mike Freeman and Joel Ross, *Programming Skills for Data Science: Start Writing Code to Wrangle, Analyze, and Visualize Data with R*, 2019. The book is available [online through the library](https://alliance-primo.hosted.exlibrisgroup.com/primo-explore/fulldisplay?docid=CP71294895890001451&context=L&vid=UW&lang=en_US&search_scope=all&adaptor=Local%20Search%20Engine&tab=default_tab&query=any,contains,programming%20skills%20for%20data%20science).
* **D'lgnazio & Klein (2020)** Refers to the course textbook, written by Catherine D'lgnazio and Lauren F. Klein, Data Feminism, 2020. The book is available [online at MIT Press](https://data-feminism.mitpress.mit.edu/)
* **Key documentation**:
   1. [Markdown documentation on GitHub](https://guides.github.com/features/mastering-markdown/#GitHub-flavored-markdown)
   2. [The Emoji Cheat Sheet](https://github.com/ikatyang/emoji-cheat-sheet)

### Preparation
1. Read: D'lgnazio & Klein (2020), the Introduction (pp. 1-19).
1. Read: Freeman & Ross (2019), chapters 1-4.
1. Download and install [Atom](https://atom.io/).
2. Download and install [Git](https://git-scm.com/).
3. Sign-up for a [GitHub](https://github.com/) user account.
3. Configure git on your computer.
4. Download and install [R](https://cran.r-project.org/) (optional for this assignment but do it now).
5. Download and install [RStudio](https://www.rstudio.com/) (optional for this assignment but do it now).

### Notes on Professional Practice
1. **Get Started Early**. For any coding project, it is very important to get started earlier because, even for expets, unwelcome surprises often arise.
1. **Plan Your Work**. Before starting to design or code, read all of the requirements of this assignment, draw some sketches, and create a todo list of the steps you need to follow. It is always a good idea to do a bit of planning before starting to design or code.
1. **Communicate with Your TA**. If you find a requirement of this assignment _ambiguous_, you should ask your Teaching Assistant or post a question on Teams. The requirements of this assignment are intended to be clear and _unambiguous_. If something is unclear, always reach out to your teaching assistant (or  project manager or team member).

### Learning Objectives
1. Demonstrate how to navigate the file system from the command line and manage files, with these and similar commands (see F&R, chap. 2):
```
pwd                                 # print working directory (to find your current location)
cd <dir>                            # change the working directory to sub-directory
cd ..                               # go to parent directory (go up)
cd <PATH>                           # go to directory specified in <path>
cd ~                                # go to your home directory 
cd ~/Documents/info201              # go to your INFO201 directory (the info201 directory must already exist)
# 
ls                                  # list files of current directory
ls -las                             # list files (show some details about the files with the flags -las)
#
mkdir <PATH>                        # make a new directory
rmdir <PATH>                        # remove a directory (use with care!)
#
cp <PATH1> <PATH2>                  # copy a file 
mv <PATH1> <PATH2>                  # move a file from one directory to another or rename a file or directory
rm <PATH>                           # remove a file or directory (use with care!)
#
less <FILENAME>                     # display the contents of a file (scroll with arrow keys; type 'q' to quit)
cat <FILENAME>                      # display the contents of a file to the terminal
#
date                                # current time and date
```
2. Set-up your directory structure for INFO-201. It should look like this (Mac OS):  
```
~/Documents/info201                  # Your root directory for INFO-201
~/Documents/info201/assignments      # Your assignments will go here, in sub-directories 
~/Documents/info201/data             # Your datasets will be saved in this directory 
~/Documents/info20/exercises         # Your weekly practice activities will go here, in sub-directories
```
3. Describe the purpose of git and GitHub (see Freeman & Ross, 2019, chap. 3).
4. Demonstrate how to manage a project using git and GitHub, with these and similar commands (see Freeman & Ross, 2019, chap. 3):
```
# Setting up basic identifying information
git config --global user.name <YOUR FULL NAME>
git config --global user.email <YOUR EMAIL ADDRESS>
#
git clone <REPO_URL>             # Copy a repo to your machine
git status                       # Check the status of a repo
git add <FILENAME>               # Add file to staging area
git add .                        # Add all files in current directory to  staging area
git git commit -m "<A MESSAGE>"  # Make changess
git push
```
5. Use markdown syntax to format document (see Freeman & Ross, 2019, chap. 4).
6. Discuss _Data Feminism_ and explain how it provides a viewpoint for critically investigating data visualizations.

## Part I: The Command Line
In Part I, you will practice working with the command line.

**Step #1**: In your directory, you will find a file named ``git-commands.md``. Open the file with Atom, which is our text editor.

**Step #2**: Following each prompt in the file ``git-commands.md``, write the line of code that you used to accomplish the task or otherwise answer the question.

**Step #3**: Save the changes to you've made to ``git-commands.md`` and then add, commit, and push your changes to GitHub.

**Note**: After completing this assignment, you can continue to add commands to this file and use it as a reference for your own work.

## Part II: Working with Markdown

In Part II, you will create a report in Markdown.

### 1. Background
Please spend **ten minutes** or more scanning all the chapters in D'lgnazio & Klein (2020). You will find many different types of data visualizations. Some types will be quite familiar to you - see, for example, the bar charts in chapter 6. Others might be new or unusual, such as the iceberg in chapter 7.

### 2 Find A Data Visualization on the Internet
Browse the web and find a data visualization that is **meaningful** to you. You might start, for example, at the [*New York Times*](http://nytimes.com) or [*Washington Post*](https://www.washingtonpost.com/) or other news source. Or, you might browse a scientific or cultural journal or website.  You should choose a visualization that was created for a specific purpose and that is credible. 

Best practice: Find several visualizations (3-5) that are appealing to you. Then, examine each one carefully and select the one that is most **meaningful** to you.

As you consider possible data visualizations, consider the following questions, which come from  D'lgnazio & Klein (2020, chap. 1):

1. **Who**: Who or what institution produced the visualization?
1. **Date**: When was it produced?
1. **Stakeholders**: Who is the audience for the visualization? And, who might be impacted, either directly or indirectly, by the visualization?
1. **Interests**: What values, goals, or interests are at stake with the visualization?
1. **Key facts**: What can be learned from the visualization?
1. **Power**: What issues, if any, are related to power are reflected in the data visualization?

**Note**: It may be difficult to answer these questions. That's okay. Nevertheless, try as best as you can to formulate specific answers.

### 3 Coding: Your Technical Requirements

Your objective is to create a report that presents your research and analysis. You will write your report using Markdown, which is a computer language for formatting text.

As you code with Markdown tags, please seek to create a professional visual appearance.

#### 3.1 Overall Requirements [Three tasks to complete]
1. Include a title.  Your title should be distinctive and it should summarize the entire report. Please do *not* create a title "A1: Tools" or something like that; instead, be concise, clear and creative.  [complete:  ]
3. Include your name and your UW e-mail address. (You are the author of the report.) [complete:  ]
4. Include the date (for exmaple, Autumn 2022) of your report. [complete:  ]

#### 3.2 Filenames and Directory Requirements [Four tasks to complete]
1. The name of the file containing your report should be ``README.md``. [complete:   ]
1. The ``README.md`` file containing your report should be located in the root directory of the repository. [complete:   ]
1. Create a new directory, named "A1-visualizations", within the "Images" directory. [complete:  ]
1. Save your data visualization imaged in the "A1-visualizations" folder. [complete:  ]

#### 3.3 Your Report: What to include? [Four tasks to complete]

First, in your own words, you should include a brief paragraph that summarizes what you did to find your data visualization and you should explain why you selected the visualization. In addition, you should include a link to your visualization. (About 100 words.) [complete: ]

Second, your report should include a description of the vizualization; that is, what specifically does the data visualization show? (About 100 words.) [complete:  ]

Third, write short responses after each of these five headings. **Please note**: You should replace the `xxx (...)` with your own written response. [complete: ]

```
**Who**: xxx (About 20 words [complete:  ])
**Date**: xxx (a year (e.g, 2021) or more specific date about when the visualization was published [complete:  ])
**Stakeholders**: xxx (About 50 words [complete:  ])
**Interests**: xxx (About 50 words [complete: ])
**Key fact**: xxx (About 50 words [complete:  ])
```
Forth, and finally, conclude your report with a brief reflection, titled, "Data Feminism: What I Learned?" (About 120 words). In this section, first, give a definition of data feminism from D'lgnazio & Klein (2020). Include the page number of the defintion. Second, given this defintion and your reading, briefly discuss one or two issues related your choosen data visualization. [complete: ])

#### 3.4 Coding Requirements [Ten tasks to complete]
In your report you **MUST** use at each of these elements at least once:

  * A top-level heading (``Heading 1``) [complete  ]
  * Three or more subheadings (e.g., ``Heading 2 ``) [complete  ]
  * An unordered list [complete  ]
  * **Bold** for emphasis [complete  ]
  * _Italics_ for emphasis [complete  ]
  * Both ***Bold and Italics*** for emphasis [complete  ]
  * An image tag to present the data visualization. Include the `ALT` tag and descriptive text for screen reader accessibility. (Note: See section 2.3 above) [complete  ]
  * A blockquote to format the definition of "Data Feminism" [complete  ]
  * Hypertext link to the website for data visualizations [complete  ]
  * An emoji -- e.g., a rocket :rocket: -- in your reflective paragraph (Note: See emoji list: [cheat-sheet](https://github.com/ikatyang/emoji-cheat-sheet)) [complete  ]
