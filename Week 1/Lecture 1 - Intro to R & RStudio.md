Welcome to DATA-LA 322!
========================================================
autosize: true
css: styles.css
## Instructor Information

### Lantz McGinnis-Brown
### Office: Online  
### Office Hours: After class or by appointment  
### Email: LantzBrown@boisestate.edu  
### Phone/Text: (208) 386-0056   

<!-- My hours are pretty flexible, if you need help, feel free to reach out,
and I'm sure we can arrange a time to chat. -->

What is Data Science?
========================================================
type: section
<img src="Data Science Venn.png", width=40% height=auto>

<div align="right">
<img src="Data Science Model.png", width=80% height=auto>
</div>

Course Description
========================================================
Study of core concepts in data science in the liberal arts, including:
* Data gathering, extraction, and cleaning
* Data mining
* Predictive modeling and machine learning

 <em> This course emphasizes practical skills for liberal arts students to examine questions of human behavior using large and complex data sets.</em>

Course Learning Outcomes
========================================================
After successful completion of this course, students will be able to:  

1. Utilize R statistical software to visualize data  

2. Analyze data using the appropriate statistical methods, including linear regression, logistic regression, and generalized linear models  

3. Utilize tree-based methods for prediction.  

4. Execute cross validation to predict outcomes and understand issues of overtraining  

5. Communicate data science processes and findings  

6. Understand the ethical implications of data science as it is applied to human subjects and their data.  

Course Format
=====
This course will include online lectures, in-class assignments, and a midterm and a final exam (both at-home and open-book).

<b>Text:</b>  
Hadley Wickham & Garrett Grolemund. (2017). [*R for Data Science: Visualize, Model, Transform, Tidy, and Import Data*](https://r4ds.had.co.nz/).

<b>Supplemental Readings:</b>  
* Yihui Xie, J.J. Allaire, & Garrett Grolemund. (2020). [*R Markdown: The Definitive Guide](https://bookdown.org/yihui/rmarkdown/).  

* RStudio's [*Cheat Sheets*](https://rstudio.com/resources/cheatsheets/).


*I may assign some other readings, but all readings will be freely available online.*

Course Requirements
=====
1. **Attendance & in-class discussion:** You are required to attend class.  
2. **Homework:** You will have homework assignments. Details will be provided in class. You are welcome to come to office hours or email me with specific questions on the homework, but I will not *check* your homework before it is due.  
3. **Exams:** The two take-home, open-book examinations will consist of a data set that you need to examine. Content will be cumulative.

# Grading:
   Attendance:  &nbsp;&nbsp; 20%/200 points (~0.67% per class)  
   Homework:    &nbsp;&nbsp;40%/400 points (~2.0% each)   
   Exam 1:      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;20%/200 points  
   Exam 2:      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;20%/200 points  
   **Total: &nbsp;&nbsp;100%/1000 points**

Accomodations
=====
Please contact the Educational Access Center (EAC) for any needed accommodations for this course. The EAC must approve accommodations before they can be implemented. To learn more about the accommodation process, visit the EAC's website at https://eac.boisestate.edu/new-eac-students/.

Academic Integrity
=====
Students in this course are expected to uphold standards outlined in the Boise State University Student Code of Conduct (http://deanofstudents.boisestate.edu/student-code-of-conduct/). Any work submitted by a student in this course for academic credit will be the student's own work.  

*Note:  While I encourage students to help each other on homework, if you submit the same document as another student, you will receive a 0%.*

Tentative Course Outline
=====
type: prompt
| Week         | Date     | Topic      | Reading | Homework Due      |
|--------------|----------|------------|---------|-------------------|
| Week 1       | 25-Aug   | Introduction to Course & R Basics  | [W & G Ch. 1 & 2](https://r4ds.had.co.nz/) |Download R & RStudio on personal computer
| Week 1       | 27-Aug   | R Basics Cont'd. | [Y,A,&G Ch. 1 & 2](https://bookdown.org/yihui/rmarkdown/garrett-grolemund.html)| Submit an intro R notebook |
| Week 2      |1-Sep |Data Visualization (ggplot2) | [W & G Ch. 3](https://r4ds.had.co.nz/) | Visualization Homework |
| Week 2      |3-Sep |Data Visualization Cont'd.   | [W & G Ch. 3](https://r4ds.had.co.nz/) | Visualization Homework

The R Statistical Software (Why R?)
=====
type: section
* R was developed by statisticians as an environment for data analysis
* R allows you to execute code line-by-line or write entire scripts.  
      - This allows you to keep a record of your analysis - which is necessary for replication
* R is free and open source
* It runs on all major operating systems
* It is easy to contribute add-ons (which leads to rapid development of new techniques that can be executed in R before other software packages)
* The Tidyverse & other packages make vast improvements on the intuitiveness and speed of the language

RStudio
=====

* Console Pane
    - Allows for line-by-line execution
    - For instance, to calculate a 17% tip on $43.92, type: 0.17 * 43.92, and hit [enter].
* Script Pane
    - File -> New File -> R Script (to make the script pane appear)
    - Allows you to write a script, save, and execute. Key for replication.
    - Color codes, catches (some) errors, helps with indentation, and can autofill text.
    - To run lines in a script, either highlight and click 'Run', or hit Control-Enter for Windows, Command-Return for Mac.
* Environment Pane
    - Allows you to see currently saved variables and data structures
* Plot Pane
    - Allows you to see your graphs
    


Key Bindings
=====
* While Rstudio is nice because it provides you some "point and click" features, it is best to learn the key bindings (or keyboard shortcuts) that you use frequently. 


* For instance, to create a new script, click: Ctrl + Shift + N (Windows) or command + shift + N (Mac).


* To see a pop-up cheatsheet of other RStudio key bindings, use Alt+Shift+K.

Creating an RStudio Project
=====
* File ->  New Project -> New Directory -> New Project


* Can be useful for keeping files and projects clean and organized
* Within a project, check out File -> New File, for some additional types of projects that you can work on within Rstudio.  You can have multiple file types within one project.


* To create a new R Notebook:
    - File -> New File -> R Notebook
    - R Notebook is a kind of R Script that uses Markdown (a simple text processing format) to mix text and code together, making code explanation and reporting easier and more intuitive. This presentation is also built with R Markdown!

Installing R Packages
=====
* Packages provide much of the functionality of R, but you need to install these packages before using them.  
* To install type: 
    - ```install.packages("tidyverse")```
    - *Note: you only have to install once.*
* Next you need to load the library
      - ```library(tidyverse)```
      - *You have to load the library every time you start a new R session*
* You can also install more than 1 package at a time:
       - ```install.packages(c("tidyverse", "palmerpenguins"))``` 
       - *c() tells R to combine values into a vector or list*
* Or, if you are more comfortable with menus, you can go to: Tools -> Install Packages, or the Packages pane in the bottom-right.
* It is useful to keep a script with all of your packages, so that if you download a fresh version of R, it is easy to reinstall all of your packages.


Changing Global/Project Options
=====
* Tools -> Global Options
* You can play in here - but as an example
   - Appearance -> Editor Theme allows you to change how the text is visible

* One possible change (particularly if you are sharing code), is to stop saving the workspace image (the R objects in your environment)
  - General/Project -> uncheck "Restore .Rdata into workspace at startup"
  -  Change "Save workspace to .Rdata on exit" to "Never" 

Git/Github
=====
* File -> New Project -> Version Control -> Git ->  Options
* GitHub allows for hosting and version control of open source projects and data 
   - It is the largest host of course code in the world
   - We may access GitHub for data
   - [Happy Git and GitHub for the useR (A Reference Book)](https://happygitwithr.com/rstudio-git-github.html)
   
Homework 1
=====
type: subsection
This assignment is pretty easy - I just want you to create an R Notebook file introducing yourself, and identifying a couple things that you are excited/nervous about related to this class. 

If you want, you can copy the example notebook I've uploaded to Blackboard. (File -> Open Files) 

Coding in R
=====
type: section

