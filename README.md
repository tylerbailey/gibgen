**Code Challenge: Gibberish Generator**
---------------------------------------

Challenge Overview
------------------

**Your response to this challenge can be used to supplement your SWEAP application.  If you plan to complete this challenge for SWEAP, ensure you meet the other minimum requirements by visiting [here](http://gecapital.com/sweap "SWEAP Home Page").  Whether you apply or not, you are welcome to fork this repository and complete as a personal project challenge.**


We are exticed taht you are intsereted in joiinng the Soawtfre Engreeniing Appsecitnerhip Prargom.  Weoclme to yuor fsrit prommarging chanellge.  Yuor chnellage is to courtsnct a prrgoam taht tekas an Enilgsh txet snirtg as iupnt and rerutns rebadale giirebbsh lkie tihs.  It dseno’t mtaetr in waht oerdr the ltteres in a wrod are, but an iproamtnt tihng is taht the frsit and lsat ltteer be in the rghit pclae. The rset can be a taotl mses and you can sitll raed it whotuit a pboerlm.  Tihs is bcuseae the huamn mnid deos not raed ervey lteter by istlef, but the wrod as a wlohe.

**The Basics:**
  
  - You may use *almost any* programming language... it's your choice.  See the supported options [here](http://ideone.com/).
  - Your program should leave the first and last letter of each word in place and scramble the rest.
  - Your program should not scamble punctuation (.,-'...etc.), numbers, or upper-case abbreviations.
  - For example gibberish, see the [/textfiles](https://github.com/sweap/gibgen/tree/master/textfiles) folder.  Two sample output files are provided: `xxx.txt.gib`

**Input/Output:**
 
  - Name your program as follows: `gibgen.xx` (where xx is variable based on the language you choose)
  - Your program should be able to read text input from a string passed into STDIN
      - `gibgen.xx "This is a String"`
      - `cat mystringfile.txt | gibgen.xx`
  - Your program should output to the console.

_Note: This challenge is based on a popular word gibberish meme. You can improve the readability by looking at a [researcher's take](http://www.mrc-cbu.cam.ac.uk/people/matt.davis/cmabridge/) on the truths/myths of this meme, but this is not required._

What to do
----------
1. [Download](http://git-scm.com/downloads) & install Git on your machine

2. <a href="https://github.com/sweap/gibgen/fork" class="btn grouped" data-method="POST" rel="nofollow" title="Fork">Fork</a> this project - Go [here](https://github.com/sweap/gibgen) and click the "Fork" button (located on the upper-right side of the screen)

2. Clone your new fork'd repository to your local machine - `git clone https://github.com/YOUR_USERNAME_HERE/gibgen.git`
3. Complete the code challenge and fill out the Quick Start & Questions in the the README (see below)
4. `git add` and `git commit` your local repository as you go
4. Push your code and README back to GitHub occasionally - `git push origin master`
5. Email [serp@ge.com](mailto:serp@ge.com) with the Commit URL to your fork'd repository that you want reviewed. It should include at least 2 files: (1) your updated README with Coding Questions answered, and (2) your program (gibgen.xx)
   - Go here: `https://github.com/YOUR_USERNAME_HERE/gibgen/commits/master`
   - Find the commit that you'd like us to review.  _The commit date must be on or before 11:59pm (central) on April 4, 2014!_
       - Click the "Browse Code ->" link for that commit
   - Copy and paste the URL into the email along with your name... it should look something like this:
       - `https://github.com/YOUR_USERNAME_HERE/gibgen/tree/73afe0c8fe2...hash.hash...e80afea72b6`

_Note: If you have any questions, email [serp@ge.com](mailto:serp@ge.com).  I will do my best to respond to any questions._

Judging Criteria
----------------

Your responses to the **Coding Questions** at the bottom of this README are the *Most Important* part of this challenge. A working, fully fault-tolerant program that we just can't break, albeit awesome, is the least important.  Why is that?  Remember, we don't expect you to be expert programmers (just yet)... We want to see how you think through a problem.  


For completion by applicant
===========================

Quick Start
-----------

* The program can be run either of the following ways
	filename | java Gibgen
	java Gibgen "my sentence to scramble"
* What programming language did you use? 
	I used Java
* Also tell us anything else the reviewer should know about your code
	I think it's pretty strait forward, I hope you don't have any issues.
	I compiled it using JDK 6.0_65 on OSX Mavericks. It was written and 
	tested in Dr.Java. 
	
	


Coding Questions
----------------

Question 1: "How did you approach the problem?" (500 words or less)

	
	My approach to the problem was to break it down into smaller pieces. After reading 
	the specs a few times to get a feel for the problem, I thought about what needed to 
	be done. I wrote methods to determine if a given character was an alphabet letter 
	and if a given string was an uppercase abbreviation. Then, I started writing a 
	method to scramble a given string. Once I felt like there were  enough pieces to 
	get a basic program running, I started on a method to read in a string from given 
	source, break it into tokens, and scramble the tokens if they were valid. After I 
	finished a rough solution, I started testing it on the given input files in the 
	repo. Comparing the output of the program with the output files, I went back and 
	refactored and cleaned up the program.

Question 2: "What was the most difficult aspect of the solution?" (500 words or less)

	I think the hardest part for me was all of the possible cases for a given token, 
	such as if it had trailing punctuation or was an upper case abbreviation with an 
	"'s" at the end. Also deciding if the program should account for things like a 
	period at the end of a sentence that didn't have a space after it. In that case 
	it would be treated like one word with punctuation inside of it instead of two 
	separate words. String parsing can be difficult because there are so many possible 
	cases depending on what you're doing. I just had to decide what was reasonable to 
	do and what wasn't.