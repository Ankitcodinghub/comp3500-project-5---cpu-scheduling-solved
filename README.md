# comp3500-project-5---cpu-scheduling-solved
**TO GET THIS SOLUTION VISIT:** [COMP3500 Project 5 – CPU Scheduling Solved](https://www.ankitcodinghub.com/product/comp3500-project-5-cpu-scheduling-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;123745&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COMP3500 Project 5 - CPU Scheduling Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
&nbsp;

<h1>1. Learning Objectives</h1>
The goal of this project is to implement a simple CPU schedule, which orchestrates three CPU scheduling policies. You will achieve the following objectives upon the completion of the project.

<ul>
<li>To design a simple CPU scheduler</li>
<li>To implement three scheduling policies in C/C++</li>
<li>To conduct scheduling simulation experiments on a Linux machine</li>
<li>Use GDB to debug your C/C++ program</li>
</ul>
&nbsp;

<h1>2. Requirements</h1>
You will implement a CPU scheduler that selects a job according to a given scheduling policy. Because the project intends to simulate a CPU scheduler, there is no need for any actual process creation, execution, or termination. When a task is scheduled, the simulator simply prints out what task is picked to run at a time. The outputs of your scheduler are similar to the Gantt chart style.

<ul>
<li>Each student should independently accomplish this project assignment. You may discuss with other students to solve the coding problems. Students should not share any project code with any other student. Collaborations among students in any form will be treated as a serious violation of the University’s academic integrity code.</li>
<li>Important! You must follow the specified output format.</li>
<li>You must write a C/C++ program on the Linux operating system.</li>
</ul>
<h1>3. Implementing a CPU Scheduler</h1>
<h2>3.1 Scheduling Policies</h2>
Your simulator should manage the following three scheduling policies. The detailed algorithms will be introduced and discussed in COMP 3500 lectures.

<ul>
<li>First Come First Serve (FCFS),</li>
<li>Round Robin or RR, and</li>
<li>Shortest Remaining Time First or SRTF).</li>
</ul>
<h2>3.2 Task Information and an Input File</h2>
The task information will be read from an input text file, the format of which is

pid arrival_time burst_time

All of fields are integer type where

<ul>
<li>pid is a unique numeric process ID</li>
<li>arrival_time is the time instance at which a task arrives</li>
<li>burst_time is the CPU time requested by a task</li>
</ul>
The time unit of arrival_time, burst_time, and interval is millisecond.

<h2>3.3 Command-line Usage</h2>
Users should run your scheduler in a command-line as:

$scheduler task_list_file [FCFS|RR|SRTF] [time_quantum]

where input_file is the file name with task information described in Section 3.2 on page 1. FCFS, RR, and SRTF are names of the scheduling policies (a.k.a., algorithms). Parameter time_quantum is only applicable to the RR policy. The FCFS policy is nonpreemptive whereas RR and SRTF are all preemptive. Table below summarize three example usages.

&nbsp;

<table width="606">
<tbody>
<tr>
<td width="198"><strong>Sample Usage </strong></td>
<td width="408"><strong>Description </strong></td>
</tr>
<tr>
<td width="198">scheduler list1 FCFC</td>
<td width="408">Simulate the FCFS policy with a task file named “input1”</td>
</tr>
<tr>
<td width="198">scheduler list2 RR 5</td>
<td width="408">Simulate RR with the “input2” task file; time quantum is set to 5.</td>
</tr>
<tr>
<td width="198">scheduler list3 SRTF</td>
<td width="408">Simulate the SRTF policy with a task file named “input3”</td>
</tr>
</tbody>
</table>
&nbsp;

<h2>3.4 System Design</h2>
<strong>Data Flow Diagram.</strong> You are suggested to start the design of your scheduler by crafting a data flow diagram, which enables you to decide what modules should be implemented and what are correlations among these modules. With the data flow diagram in place, you are expected to have a clear picture on key data structures used in your scheduler. In the data-flow-diagram design phase, please ignore any issue related to algorithm design (e.g., time-driven simulation, scheduling policies).

<strong>Loading Input File.</strong> After the simulator reads a task information list from an input text file, all the task information should be stored in a task list (e.g., an array, a dynamic array, or a linked list). Then, the simulator schedules tasks according to a scheduling policy specified in the command-line.

<strong>Time-Driven Simulation.</strong> Your simulator manages tasks in a time-driven manner. More specifically, at each time unit (a.k.a., time slot), your simulator inserts any newly arrived task into the ready queue, followed by invoking the scheduler to choose an appropriate task from the ready queue. When a task is elected to run, the simulator prints out a message indicating the process ID of a task running in this time slot. If no task is running (i.e., the ready queue is empty) during the current time unit, the simulator prints out an “idle” message. Before advancing to the next time unit, the simulator should update all necessary changes in the running task and the ready queue status.

&nbsp;

<h2>3.5 Output and Statistical Information</h2>
Your simulator will be applied to compare the performance among the three scheduling policies. The scheduler is expected to compute the following statistical information referred to performance metrics. You will learn these metrics in our lectures. Please refer to Section 6 on page 4 for a sample output.

<ul>
<li>average waiting time</li>
<li>average response time</li>
<li>average turnaround time</li>
<li>overall CPU usage</li>
</ul>
<h2>3.6 Suggested Functions</h2>
You are recommended to implement the following functions.

<ul>
<li><strong>A command-line parser.</strong> Please refer to the command-line parser in os161 as an example.</li>
<li><strong>Three scheduling algorithms.</strong> Each scheduling policy should be implemented in a dedicated function.</li>
<li><strong>Read an input file.</strong> This function is responsible for loading a task information list from an input file into your simulator.</li>
<li><strong>Print statistic information. </strong>All the performance measures (e.g., average waiting time) must be displayed upon the completion of a simulation.</li>
<li><strong>Error handler. </strong>If an input command doesn’t follow the specified format, the error handler must handle all types of input errors.</li>
</ul>
<strong>&nbsp;</strong>

<h1>4. Programming Requirements</h1>
<h2>4.1 Programming Environment</h2>
Write your simulated virtual memory system in either C or C++.&nbsp; Compile and run your system using the gcc or g++ compiler on a Linux box (either in the computer labs in Shelby, your home Linux machine, a Linux box on a virtual machine, or using an emulator like Cygwin).

&nbsp;

<h2>4.2 Function-Oriented Approach</h2>
You are <em>strongly suggested</em> to use a structure-oriented (a.k.a., function-oriented) approach for this project. In other words, you will need to write function definitions and use those functions; you can’t just throw everything in the main() function. A well-done implementation will produce a number of robust functions, many of which may be useful for future programs in this project and beyond.

Remember good design practices include:

<ul>
<li>A function should do one thing, and do it well</li>
<li>Functions should NOT be highly coupled</li>
</ul>
<strong>&nbsp;</strong>

<h2>4.3 File Names</h2>
You will lose points if you do not use the specific program file name, or do not have a comment block on every source code file you hand in.

&nbsp;

<h2>4.4 Usability Concerns and Error-Checking</h2>
You should appropriately prompt your user and assume that they only have basic knowledge of the system. You should provide enough error-checking that a moderately informed user will not crash your system.&nbsp; This should be discovered through your unit-testing.&nbsp; Your prompts should still inform the user of what is expected of them, even if you have error-checking in place.

&nbsp;

<h1>5. Separate Compilation</h1>
You must use separate compilation and create a makefile for this project.

<strong>&nbsp;</strong>

<strong>5.1 What’s Make?&nbsp; </strong>

Make is a program that looks for a file called “makefile” or “Makefile”, within the makefile are variables and things called dependencies. There are many things you can do with makefiles, if all you’ve ever done with makefiles is compile C or C++ then you are missing out. Pretty much anything that needs to be compiled (postscript, java, Fortran), can utilize makefiles.

<h2>5.2 Format of Makefiles — Variables</h2>
First, lets talk about the simpler of the two ideas in makefiles, variables. Variable definitions are in the following format:

VARNAME = Value

So let’s say I want to use a variable to set what compiler I’m going to use. This is helpful b/c you may want to switch from cc to gcc or to g++. We would have the following line in our makefile

CC = gcc

This assigns the variable CC to the string “gcc”. To expand variables, use the following form:

${VARNAME}

So to expand our CC variable we would say:

${CC}

<em>&nbsp;</em>

<h2>5.3 Format of Makefiles — Dependencies</h2>
Dependencies are the heart of makefiles. Without them nothing would work. Dependencies have the following form:

dependecy1: dependencyA dependencyB … dependencyN&nbsp;&nbsp;&nbsp;&nbsp; command for dependency1

Check out the following links for more information on makefiles:

<a href="https://www.gnu.org/software/make/manual/html_node/Introduction.html">https://www.gnu.org/software/make/manual/html_node/Introduction.html </a>

<strong>&nbsp;</strong>

<h1>6. Sample Input and Output</h1>
Suppose an input task file is called “task.list”, your scheduler should run as follows to simulate the three scheduling policies.

&nbsp;

%more task.list

<ul>
<li>0 10</li>
<li>0 9</li>
<li>3 5</li>
<li>7 4</li>
<li>10 6</li>
<li>10 7</li>
</ul>
&nbsp;

%scheduler

Usage: scheduler task_list_file [FCFS|RR|SRTF] [time_quantum]

&nbsp;

%scheduler task.list FCFS

Scheduling Policy: FCFS

There are 6 tasks loaded from “task.list”. Press any key to continue …

==================================================================

&lt;time 0&gt; process 1 is running &lt;time 1&gt; process 1 is running &lt;time 2&gt; process 1 is running

&lt;time 3&gt; process 1 is running

&lt;time 4&gt; process 1 is running

&lt;time 5&gt; process 1 is running

&lt;time 6&gt; process 1 is running

&lt;time 7&gt; process 1 is running

&lt;time 8&gt; process 1 is running

&lt;time 9&gt; process 1 is running &lt;time 10&gt; process 1 is finished…

&lt;time 10&gt; process 2 is running

&lt;time 11&gt; process 2 is running

&lt;time 12&gt; process 2 is running

&lt;time 13&gt; process 2 is running

&lt;time 14&gt; process 2 is running

&lt;time 15&gt; process 2 is running

&lt;time 16&gt; process 2 is running

&lt;time 17&gt; process 2 is running

&lt;time 18&gt; process 2 is running &lt;time 19&gt; process 2 is finished…

&lt;time 19&gt; process 3 is running

&lt;time 20&gt; process 3 is running

&lt;time 21&gt; process 3 is running

&lt;time 22&gt; process 3 is running

&lt;time 23&gt; process 3 is running &lt;time 24&gt; process 3 is finished…

&lt;time 24&gt; process 4 is running

&lt;time 25&gt; process 4 is running

&lt;time 26&gt; process 4 is running

&lt;time 27&gt; process 4 is running &lt;time 28&gt; process 4 is finished…

&lt;time 28&gt; process 5 is running

&lt;time 29&gt; process 5 is running

&lt;time 30&gt; process 5 is running

&lt;time 31&gt; process 5 is running

&lt;time 32&gt; process 5 is running

&lt;time 33&gt; process 5 is running &lt;time 34&gt; process 5 is finished…

&lt;time 34&gt; process 6 is running

&lt;time 35&gt; process 6 is running

&lt;time 36&gt; process 6 is running

&lt;time 37&gt; process 6 is running

&lt;time 38&gt; process 6 is running

&lt;time 39&gt; process 6 is running

&lt;time 40&gt; process 6 is running &lt;time 41&gt; process 6 is finished…

&lt;time 41&gt; All processes finish ……

============================================================

Average waiting time:&nbsp;&nbsp;&nbsp; 14.17

Average response time:&nbsp;&nbsp; 14.17

Average turnaround time: 21.00

Overall CPU usage:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 100.00%

============================================================

<strong>&nbsp;</strong>

&nbsp;

%scheduler

Usage: scheduler task_list_file [FCFS|RR|SRTF] [time_quantum]

&nbsp;

%scheduler task.list SRTF

Scheduling Policy: SRTF

There are 6 tasks loaded from “task.list”. Press any key to continue …

==================================================================

&lt;time 0&gt; process 2 is running

&lt;time 1&gt; process 2 is running

&lt;time 2&gt; process 2 is running

&lt;time 3&gt; process 3 is running

&lt;time 4&gt; process 3 is running

&lt;time 5&gt; process 3 is running

&lt;time 6&gt; process 3 is running

&lt;time 7&gt; process 3 is running

&lt;time 8&gt; process 3 is finished…

&lt;time 8&gt; process 4 is running

&lt;time 9&gt; process 4 is running

&lt;time 10&gt; process 4 is running

&lt;time 11&gt; process 4 is running

&lt;time 12&gt; process 4 is finished…

&lt;time 12&gt; process 2 is running

&lt;time 13&gt; process 2 is running

&lt;time 14&gt; process 2 is running

&lt;time 15&gt; process 2 is running

&lt;time 16&gt; process 2 is running

&lt;time 17&gt; process 2 is running

&lt;time 18&gt; process 2 is finished…

&lt;time 18&gt; process 5 is running

&lt;time 19&gt; process 5 is running

&lt;time 20&gt; process 5 is running

&lt;time 21&gt; process 5 is running

&lt;time 22&gt; process 5 is running

&lt;time 23&gt; process 5 is running

&lt;time 24&gt; process 5 is finished…

&lt;time 24&gt; process 6 is running

&lt;time 25&gt; process 6 is running

&lt;time 26&gt; process 6 is running

&lt;time 27&gt; process 6 is running

&lt;time 28&gt; process 6 is running

&lt;time 29&gt; process 6 is running

&lt;time 30&gt; process 6 is running

&lt;time 31&gt; process 6 is finished…

&lt;time 31&gt; process 1 is running

&lt;time 32&gt; process 1 is running

&lt;time 33&gt; process 1 is running

&lt;time 34&gt; process 1 is running

&lt;time 35&gt; process 1 is running

&lt;time 36&gt; process 1 is running

&lt;time 37&gt; process 1 is running

&lt;time 38&gt; process 1 is running

&lt;time 39&gt; process 1 is running

&lt;time 40&gt; process 1 is running &lt;time 41&gt; process 1 is finished…

&lt;time 41&gt; All processes finish ……

============================================================

Average waiting time:&nbsp;&nbsp; 10.50

Average response time:&nbsp; 9.00

Average turnaround time:17.33

Overall CPU usage : 100.00 %

============================================================

<strong>&nbsp;</strong>

&nbsp;

%scheduler

Usage: scheduler task_list_file [FCFS|RR|SRTF] [time_quantum]

%scheduler task.list RR 4

Scheduling Policy: RR

There are 6 tasks loaded from “task.list”. Press any key to continue …

==================================================================

&lt;time 0&gt; process 1 is running

&lt;time 1&gt; process 1 is running

&lt;time 2&gt; process 1 is running

&lt;time 3&gt; process 1 is running

&lt;time 4&gt; process 2 is running

&lt;time 5&gt; process 2 is running &lt;time 6&gt; process 2 is running &lt;time 7&gt; process 2 is running

&lt;time 8&gt; process 3 is running

&lt;time 9&gt; process 3 is running

&lt;time 10&gt; process 3 is running

&lt;time 11&gt; process 3 is running

&lt;time 12&gt; process 1 is running

&lt;time 13&gt; process 1 is running

&lt;time 14&gt; process 1 is running

&lt;time 15&gt; process 1 is running

&lt;time 16&gt; process 4 is running

&lt;time 17&gt; process 4 is running

&lt;time 18&gt; process 4 is running

&lt;time 19&gt; process 4 is running

&lt;time 20&gt; process 4 is finished…

&lt;time 20&gt; process 2 is running

&lt;time 21&gt; process 2 is running

&lt;time 22&gt; process 2 is running

&lt;time 23&gt; process 2 is running

&lt;time 24&gt; process 5 is running

&lt;time 25&gt; process 5 is running

&lt;time 26&gt; process 5 is running

&lt;time 27&gt; process 5 is running

&lt;time 28&gt; process 6 is running

&lt;time 29&gt; process 6 is running

&lt;time 30&gt; process 6 is running

&lt;time 31&gt; process 6 is running

&lt;time 32&gt; process 3 is running

&lt;time 33&gt; process 3 is finished…

&lt;time 33&gt; process 1 is running

&lt;time 34&gt; process 1 is running

&lt;time 35&gt; process 1 is finished…

&lt;time 35&gt; process 2 is running

&lt;time 36&gt; process 2 is finished…

&lt;time 36&gt; process 5 is running

&lt;time 37&gt; process 5 is running

&lt;time 38&gt; process 5 is finished…

&lt;time 38&gt; process 6 is running

&lt;time 39&gt; process 6 is running

&lt;time 40&gt; process 6 is running &lt;time 41&gt; process 6 is finished…

&lt;time 41&gt; All processes finish ……

============================================================

Average waiting time:&nbsp;&nbsp; 22.00 Average response time:&nbsp; 8.33

Average turnaround time:28.83

Overall CPU usage:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 100.00%

============================================================

<strong>&nbsp;</strong>

<h1>7. Project Report</h1>
Write a project report that explains how you design and implement your virtual memory manager. Your report must address all of the questions. Your report is worth 15 points.

<strong>&nbsp;Important! </strong>&nbsp;Your project report should provide sample input and output from your scheduler.

&nbsp;

<h2>7.1 (6 points) Solution Description</h2>
You must describe your solutions with good sample input and output to show users what your scheduler is doing.

<ul>
<li>How did you separate scheduling mechanism from scheduling policies?</li>
<li>How did implement the three scheduling algorithms?</li>
<li>How did you calculate waiting times?</li>
<li>How did you calculate response times?</li>
<li>How did you calculate turnaround times?</li>
<li>How did you implement the command-line parser?</li>
</ul>
&nbsp;

<strong>7.2</strong><strong> (6 points) Generality and Error Checking </strong>(1) How general is your solution?

<ul>
<li>How easy would it be to add a new scheduling policy into your scheduler?</li>
<li>Does your program offer input error checking?</li>
</ul>
&nbsp;

<h2>7.3 (3 points) Miscellaneous factors</h2>
<ul>
<li>Is your code elegant?</li>
<li>How innovative is your solution? Did you try any ideas not suggested here?</li>
<li>Did you document all outside sources?</li>
</ul>
<strong>&nbsp;</strong>

<h1>8. Deliverables</h1>
<h2>8.1 Final Submission</h2>
Your final submission should include:

<ul>
<li>A project report (see also Section 7)</li>
<li>A copy of the complete source code of your CPU scheduler</li>
<li>Makefile (see also Section 5 on page 3)</li>
</ul>
<strong>&nbsp;Important! </strong>&nbsp;You must submit a single compressed file (see Section 8.2) as a .tgz file, which includes both a project report, source code, and Makefile.

<strong>&nbsp;</strong>

<h2>8.2 A Single Compressed File: proejct5.tgz</h2>
Now, submit your tarred and compressed file named proejct5.tgz through Canvas. You must submit your single compressed file through Canvas (no e-mail submission is accepted).

&nbsp;

<strong>8.3 What happens if you can’t complete the project? </strong>

If you are unable to complete this project for some reasons, please describe in your final design document the work that remains to be finished. It is important to present an honest assessment of any incomplete components.

<strong>&nbsp;</strong>

<h2>11. Rebuttal period</h2>
<ul>
<li>You will be given a period a week (7 days) to read and respond to the comments and grades of your homework or project assignment. The TA may use this opportunity to address any concern and question you have. The TA also may ask for additional information from you regarding your homework or project.</li>
</ul>
