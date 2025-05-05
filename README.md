# operating-systems-exercise-1-system-calls-basic-i-o-solved
**TO GET THIS SOLUTION VISIT:** [Operating Systems Exercise 1-System Calls, Basic I/O Solved](https://www.ankitcodinghub.com/product/operating-systems-exercise-1-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;99216&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Operating Systems Exercise 1-System Calls, Basic I\/O Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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

<div class="kksr-stars-active" style="width: 0px;">
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
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="section">
<div class="layoutArea">
<div class="column">
<ol start="0">
<li>Part 1In this question we will implement a C application that appends content from a file to another. The application should receive the buffer size (in bytes), source file path and target file path as command line arguments. By default, the application does not create a target file if such does not exist, unless the -f option was specified.
<ol>
<li>Read the manual page for the following System Calls i.e. execute: man 2 read
<ol>
<li>READ(2)</li>
<li>RENAME(2)</li>
<li>OPEN(2), and Carefully read about the following option flags:O_RDONLY, O_WRONLY, O_CREAT,O_APPEND O_TRUNC, O_EXCL.</li>
<li>CLOSE(2)</li>
</ol>
</li>
<li>Read the manual page for the following C Library Calls a. PERROR(3)b. PRINTF(3)c. EXIT(3)</li>
<li>Complete the application in the provided ex1.c file (missing parts are marked with</li>
</ol>
</li>
</ol>
</div>
</div>
<div class="layoutArea">
<div class="column">
//TODO).

</div>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="section">
<div class="layoutArea">
<div class="column">
Execution output examples:

$ ./ex1

Invalid number of arguments Usage:

ex1 [-f] BUFFER_SIZE SOURCE DEST

$ ./ex1 /etc/passwd /tmp/passwd

Invalid number of arguments Usage:

ex1 [-f] BUFFER_SIZE SOURCE DEST

$ ./ex1 4096 /etc/passwd /tmp/passwd

Unable to open destination file for writing: No such file or directory

$ ./ex1 -f 4096 /etc/passwd /tmp/passwd

Content from file /etc/passwd was successfully appended to /tmp/passwd

$ ./ex1 -f 4096 /tmp/passwd /etc/passwd

Unable to open destination file for writing: Permission denied

$ ./ex1 4096 /etc/password /tmp/passwd

Unable to open source file for reading: No such file or directory

Output Requirements &amp; Testing:

In order to apply a uniform testing procedure to your submissions, your program must output one of the following types of messages (precisely and case-sensitive):

</div>
</div>
<div class="layoutArea">
<div class="column">
• • • • • • • •

Or one

</div>
<div class="column">
Unable to open source file for reading

Unable to open destination file for writing

Unable to append to destination file

Unable to append buffer content to destination file

Unable to read source file

Unable to close source file

Unable to close destination file

Content from file &lt;source_file&gt; was successfully appended to &lt;destination file&gt;

of the various arguments parsing errors, as described in the examples above.

</div>
</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="section">
<div class="layoutArea">
<div class="column">
Note that all console outputs are expected to end with a newline as shown in the examples above.

Please notice that the output of your program will be checked, as well as the contents of the file that was created during the append process, if such append takes place.

Guidelines

<ul>
<li>● &nbsp;Use the manuals. Chapters 2 &amp; 3 are your friends</li>
<li>● &nbsp;Make sure to always close the files you are using</li>
<li>● &nbsp;Always check system calls return value for errors. ALWAYS.</li>
<li>● &nbsp;You are not allowed to use any external / C-Library code that copies files, if you arenot sure if you are allowed to use something, ask in the forum.</li>
<li>● &nbsp;Your program must finish executing with EXIT_SUCCESS only when there were no errors(otherwise it must finish executing with EXIT_FAILURE after printing a helpful message).</li>
<li>● &nbsp;Do not change function signatures, if provided.</li>
<li>● &nbsp;Hint: the 4 system calls and 3 libc calls mentioned above are all you need toimplement this part of the exercise successfully.Using Docker for Smoke Testing</li>
</ul>
<ul>
<li>The VM is installed with Docker software (more on that later in the semester).</li>
<li>When being graded, your solution will be tested in a container identical to the one thatwill be built using the supplied Dockerfile.</li>
<li>There are two smoke tests (sanity checks) to this exercise. You can explore the’EX1/check_submission/do_not_change’ folder for more details</li>
</ul>
o Test1 – tests a standard scenario: source file and destination file exist and not

empty

o Test2 – tests a scenario in which the destination file is missing (and there is no ‘-f’

flag) • Usage:

o You’re given EX1 folder, containing:

<ul>
<li>▪ &nbsp;A ‘check_submission’ folder, which contains two tests (Test0, Test1) anda Python script to execute it (check_submission.pyc).</li>
<li>▪ &nbsp;A skeleton file ‘ex1.c’</li>
</ul>
o Do not move ANY of the files inside check_submission, or you won’t be able to use our tests.

o You should edit ‘ex1.c’ with your solution.

o Each time you want to test your final submission file (zip file):

<ul>
<li>▪ &nbsp;Open a terminal and go the EX1/check_submission.</li>
<li>▪ &nbsp;copy your submission file (ex1-YOUR_ID.zip) to your machine (anywhereyou want)</li>
</ul>
</div>
</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="section">
<div class="layoutArea">
<div class="column">
▪ Execute ‘python check_submission.pyc &lt;full path to your submission file&gt;’. for example:

▪ If the two tests pass, you’ll get:

</div>
</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="section">
<div class="layoutArea">
<div class="column">
Part 2 (24 points)

We will now examine the performance of our program from part 1.

<ol>
<li>Create a 5MB file using the following command:</li>
<li>Run your program on this file, preceded with the time(1) command, using the following buffer sizes: 100, 200, 400, 800, 1600, 3200, 6400, 12800, 25600, 51200</li>
<li>Draw a graph (using Google Sheets or Microsoft Excel) with 3 series: Real, User, Sys. The series should show the time each run takes (in milliseconds) [Y axis], as a function of the buffer size [X axis]</li>
<li>Explain the graph:
<ul>
<li>● &nbsp;What is the meaning of Real, User and Sys (use Google)?
<pre>         _____________________________________________________________________
         _____________________________________________________________________
         _____________________________________________________________________
</pre>
</li>
<li>● &nbsp;Why don’t Sys and User sum up to Real? _____________________________________________________________________ _____________________________________________________________________ _____________________________________________________________________</li>
<li>● &nbsp;Why isn’t Real a straight line, parallel to the X axis?___________________________________________________________________ ___________________________________________________________________ ___________________________________________________________________</li>
</ul>
</li>
<li>Hypothetically, if we change the append_file in part 1 to print out to the screen a message each time we read buffer_size bytes, will the running time change significantly?</li>
</ol>
● IMPORTANT: Do not make this change. Submission with this change will result in 0 points for this question!

<pre>      _______________________________________________________________________
      _______________________________________________________________________
      _______________________________________________________________________
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
dd if=/dev/zero of=/tmp/test.5mb bs=1M count=5

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
$ time ./ex1 -f 51200 /tmp/test.5mb /tmp/test.5mb_dest File /tmp/test.5mb was copied to /tmp/test.5mb_dest

Real 0m0.004s

User 0m0.000s Sys 0m0.000s

</div>
</div>
</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="section">
<div class="layoutArea">
<div class="column">
Part 3 (40 points)

Answer ‘Homework 1 Quiz’ in Moodle (10 T/F questions, 4 points each).

</div>
</div>
</div>
</div>
