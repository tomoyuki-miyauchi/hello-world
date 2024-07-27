---
layout: page
title: "git memo"
permalink: /docs/git-memo
---

# ソフトウェア工学 2024

Summarize what I've learned in software engineering on this page.

## About software and software engineering

### Software definition
- A set of insruction words that, when executed, provide the required characteristics, functions, and performance.
- Data structures that allow programs to handle information appropriately.
- Information describing the operation and use of the program
### Software features
- Must adanpt to meet the needs of new environments and technologies.
- Must be enhanced to meet new business demand
- Must be extended to interoperate with more modern systems and databases.  

***
### Definition of Software Engineering
&nbsp; "The application of a sustematic, disciplined, and quantifiable approach to software development, operation, and maintenance, that is the application of engineering to software."  
***

Software engineering is needed for the following reasons.
1. Large scale and Complexity
2. Lack of IT personel
3. Social and required missions
4. Increased uncertainty

***
## System Development Flow  
Requirement Definition -> Design -> Modification -> Testing

### requirements definition
- System objectives
- System overview
- System function
- System configuration (system configuration diagram, software block diagram)
- Target performance
- Interface specifications with other system
- Operational considerations
- Restrictions
- Expandability
- Development schedule
- Development system
- Deliverables

### Design
- From requirements definition document to design document
- Reduce to a specification at a level where coding can be done
  - Classes, Modules
- WBS (Work Breakdown Structure)

### Modification
- System construction according to design decuments in-house - - - In-house production (in-house development)
  - Some functions may be purchased as a package of function or outsourced
- Procurement
  - Outsource development
  - Include source code in deliverables or not
    - If included
      - Maintenance can be done in-house
    - If not included
      - Maintenance must be outsourced

### Testing & Debug
- No software without bugs (should be considered)
- Ideally, software should be tested in advance to detect and deal with bugs as early as possible
- It's impossible to test everything (man-hours are limited)
  - Which parts of the software should be tested?
  - How much to test?
    - Do we debug all the way into dasses and functions?

***
## What is "Project"?
Features of project
- Definite period or characteristic
  - The kind of work that always has an end
- Uniqueness
  - The kind of work that achiebes a unique goal

### Forcasting or Backcasting
- Forcasting
  - Input perspective (how much did you do?)
  - Advancing to the goal in order from where we stand now
  - There is a possibility that the goal will not be reached
  - May reach the goal and far from it
- Backcasting
  - Output perspective (what was accomplished?)
  - Plan what is needed to achieve the goals you hhave set and work toward achieving them
  - Need to set clear goals
  - Need to consider the path toward the goal

<strong>Project -> Backcasting</strong>

## Software Evaluation
Software Evaluation = Measuring value

1. Quantity of code (number of steps)
  - Number of lines of source code in terms of specific language (total number of steps)
  - If multiple languages are mixed, they need to be converted

2. Quantity of code (object capacity)
  - Smaller size is better for embedded software

3. Function point (FP) method
  - The system size can be estimated when user requirements are defined and necessary function are ientified befor entering the programming phase
    - Rough estimate -> design specifications -> re-estimate -> estimate system size
    - The system scale can also be used as an indicator for investment decision making, such comparing the scale of different systems when procuring a system, and whether to develop a new sysstem or purchase a new one  

FP balue = base value * (0.65 + adjusted value / 100)
Cost = FP value * work unit * conversion value

4. Ease of use
  1) Screen visibility
  2) Operability
  3) INput assistance
  4) Compatibility
  5) Guidance

### Bug Incidence Rate
Number of bugs per step (number of lines of code excluding openings)

Example)
100 tests are performed on 100 steps of software and 10 bugs are generated  
<strong>Bug occurrence rate1 = 10 (bugs) / 100 (steps) = 0.1 (bugs / steps)</strong>  
Additional 50 tests are performed and 5 bugs occur
<strong>Bug rate2 = 15 (bugs) / 100 (steps) = 0.15 (bugs / steps)</strong>  

Bug incidence rate is one indicator of software quality evaluation

## Development process
### Waterfall development process
- Easy to manage progress, clear deliverables
- There is a risk of concentration of work on the back end of the process

### Spiral model
- Program development is divided into small phases
- Demonstration by prototype->feedback for each phase
- There is a risk of unexpected workload in prototyping

### Iterative development process
- Software is divided into functional units, which are managed in units called “iterations
Advantages
  - Easy to incorporate customer requirements because software is completed in parts
  - Partial delivery is possible
Disadvantages
  - Increased work and management tasks due to division
  - Difficult to see the whole picture
  - For a system that operates in a batch, it becomes meaningless to split the system.

### Agile Process
- Consider “tolerance” of engineers
- Priority is given to providing software that works in an optimal manner by responding to changes and eliminating waste
- Delays decisions as long as possible” and ‘delivers as quickly as possible,’ which were not envisioned in the waterfall development process
- Eliminate waste by increasing motivation and learning effectiveness

#### The Value of Agile
- Individuals and interactions rather than processes and tools
- Moving software rather than easy-to-understand documentation
- Collaboration with customers rather than contractual gamesmanship
- Adaptability to change rather than rigid adherence to a plan

#### Agile Concepts
- Acceptance of change
- Fast cycles/frequent deliveries
- Simple design
- Refactoring
- Pair programming
- Retrospective
- Tacit knowledge
- Test-driven development

#### 12 Principles of Agile Development
1. reaching customer satisfaction through early and continuous delivery of software is paramount.
2. be willing to change requirements, even at the end of the development process. Agile processes control change for the customer's competitive advantage.
3. deliver software in cycles of weeks to months, the shorter the better.
4. business people and developers must collaborate daily throughout the project.
5. Organize the project around highly motivated developers. Give them the necessary environment and support, and trust that they will complete the task.
6. the most efficient and effective means of communication, both inside and outside the development team, is face to face
7. working software is the primary means of tracking progress.
Agile software development encourages sustainable development. Funders, developers, and users should always keep a steady pace. 9. agility is improved by constant attention to technical competence and good design.
10. brevity in not doing what is unnecessary is essential.
11. modern architectures, requirements, and designs emerge from self-organized teams.
12. Periodically, teams harmonize and adjust the way they develop, thinking of ways to be more effective.

Development methods are one-size-fits-all, and it is essential to have project management skills to identify and determine the most effective method depending on the situation and requirements. In addition, there are many hybrid methods that combine these methods.


## WBS (Work Breakdown Structure)
<strong>WBS: A hierarchical elemental decomposition of the work performed by the project team to achieve the project goals and produce the required elemental deliverables, with the elemental deliverables as the main elements.</strong>  
Merit:
- Scope clarification
- Identify the work to be done
- Overall management and work plan are clarified
- During project implementation, only execute according to the WBS

### How to create WBS
- Clarify the Scope
  - Top-down approach
  - Backcasting
- Grouping large tasks
  - Example: data collection, data analysis, visualization
- Consider interrelationships among grouped tasks
  - Analyze after data collection
  - ≠Do not collect data after analyzing data
- Identify the tasks in each grouping
  - No duplication of work


## UML


***
## About git

&nbsp; git is a distributed version control system, originally software for open source software management.  
&nbsp; git has the following advantages:
- A history of changes is kept
- Can go back to the point where you made the change
- Can be edited jointly with others


### Repository
&nbsp; git has local and remote repositories in the project folder managed by git

<dl>
    <dt><strong>Local repository</strong></dt>
        <dd>&nbsp; Execution environment for individual projects.</dd>
        <dd>&nbsp; Local repository is a copy of the entire project's and codebase that resides on a developer's machine.</dd>
        <dd>&nbsp; It allows developers to work offline.</dd>
</dl>

<dl>
    <dt><strong>Remote repository</strong></dt>
        <dd>&nbsp; Shared management location</dd>
        <dd>&nbsp; Remote repository serv es as a central hub where developers can collaborate and share their work with others.</dd>
        <dd>&nbsp; It enables team members to synchronize their changes and provides backup and visibility for the project.</dd>
</dl>


### Commit

&nbsp; Use "Commit" to record file creation/modification/deletion.  
&nbsp; Commit has the folloeing characteristics:  

- When manipulating a file, it must be known "when","who","what", and "how" the file was manipulated, and when committing the file, "how" the file was manipulated should be described.
- There can be one or more target files to commit
- The user is free to determine the unit of commit

![alt text](git_file_version.jpg)

### Branch

&nbsp; "Branch" alows work to be branched out. This allows for collaboration and transition work

![alt text](branch.png)

### Flow in local repository

![alt text](flow_in_local.jpg)

#### Worktree  
- There are three states of files  
 1.untracked  
  &emsp; The state of files not tracked by git  
 2.unmodified  
  &emsp; The state of files tracked by git but not corrected  
 3.modifieed  
  &emsp; The state of files tracked and corrected by git

#### Staging area
- Register files tracted by git  
- staged: The state of files registered in staging area  

#### Git directory
- Register changes by "commit"  
- <strong>In principle, "commit" can't be changed or deleted</strong>  
&emsp; &nbsp; (Changes and deletion of "commit" are also recorded)  
- Committed files become unmodified  

### Flow in remote repository
- Reflect changes committed in local repository to remote repository ("git push")  
- Reflect content from remote repository to local repository ("git pull")  

![alt text](remote_repository.drawio.png)

## Git Commands

The main commands used in git are following:

<details><summary><strong>Setting/confirmation system</strong> </summary>
<dl>
    <dt><strong>git init</strong></dt>
        <dd>Initialize/set up git</dd>
    <dt><strong>git status</strong></dt>
        <dd>Display work tree status</dd>
    <dt><strong>git config</strong></dt>
        <dd>Check/change around settings</dd>
    <dt><strong>git log</strong></dt>
        <dd>Show log</dd>
        <dd>'--oneline' listing of only one line of a commit message</dd>
    <dt><strong>git diff</strong></dt>
        <dd>Show file diffs</dd>
</dl>
</details>


<details><summary><strong>Commit system</strong> </summary>
<dl>
    <dt><strong>git add</strong></dt>
        <dd>Add to staging area</dd>
    <dt><strong>git commit</strong></dt>
        <dd>Commit execution</dd>
</dl>
</details>


<details><summary><strong>Correction system</strong> </summary>
<dl>
    <dt><strong>git commit --amend --no-edit</strong></dt>
        <dd>Commit correction</dd>
    <dt><strong>git checkout</strong></dt>
        <dd>Recover deleted files, restore past commits, etc.(if undo changes are in staging area/index)</dd>
    <dt><strong>git reset</strong></dt>
        <dd>Reset commit</dd>
    <dt><strong>git revert</strong></dt>
        <dd>Commit to "cancel commit changes"</dd>
    <dt><strong>git rm</strong></dt>
        <dd>Delete files and index information</dd>
</dl>
</details>


<details><summary><strong>Remote system</strong> </summary>
<dl>
    <dt><strong>git clone</strong></dt>
        <dd>Copy repository</dd>
    <dt><strong>git pull</strong></dt>
        <dd>Synchronization of remote repositories</dd>
    <dt><strong>git push</strong></dt>
        <dd>Upload changes</dd>
    <dt><strong>git request-pull</strong></dt>
        <dd>Pull request : Change request</dd>
    <dt><strong>git remote</strong></dt>
        <dd>Remote repository setting</dd>
</dl>
</details>


<details><summary><strong>Branch system</strong> </summary>
<dl>
    <dt><strong>git branch</strong></dt>
        <dd>Branch creation</dd>
    <dt><strong>git checkout</strong></dt>
        <dd>Branch switching</dd>
    <dt><strong>git merge</strong></dt>
        <dd>Branch consolidation</dd>
        <dd>'--ff-only:fast forward only' marge into unchanged destination branch</dd>
    <dt><strong>git clone</strong></dt>
        <dd>Copy repository</dd>
    <dt><strong>git push</strong></dt>
        <dd>Upload changes</dd>
</dl>
</details>