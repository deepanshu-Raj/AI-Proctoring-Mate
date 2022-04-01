<h1 align="center">AI-Proctoring-Mate</h1>
<p align="center">

  <img src="https://user-images.githubusercontent.com/54600788/161250273-16048a4d-29aa-45dd-8c67-9ff206aa091f.png" height=350 width=600>

</p>

<p><a href="https://hack36.com" > <img src="http://bit.ly/BuiltAtHack36" height=20px> </a></p>


## Introduction:
  
<p><b>AI-Proctoring-Mate</b> is an <b>end-to-end Examination Portal</b>, with <b>AI-proctored student's Interface</b> for taking the quiz/test, and a <b>Web app for Teachers and Online Quiz creators</b> for creating quizzes, viewing responses, and sending Feedback to students on the basis of their performance in the Test/Quiz.</p>
  
## Demo Video Link:
  <a href="https://drive.google.com/file/d/1DCIg-qzuCiQ5d_pwO4xyPGxk1fIBsp0h/view?usp=sharing">AI-Proctoring-Mate Video</a>
  
## Presentation Link:
  <a href="https://drive.google.com/file/d/1Mz-T13XT33YgwE-34xKqBQ-fnPwoy4Y_/view?usp=sharing"> AI-Proctoring-Mate PPT </a>
  
  
## Table of Contents:

### Technology Stack:

  - Machine Learning
  - Tkinter
  - Selenium
  - HTML,CSS,Bootstrap,JS
  - ApexChart.js
  - Django
  - SQlite3
  

### Contributors:

Team Name: **Apunich bhagwan ha**

* <code>[Deepanshu Raj](https://github.com/deepanshu-Raj)</code>
* <code>[Sidhant Agarwal](https://github.com/sidhantagar)</code>
* <code>[Vivek Rai](https://github.com/Blazer-007)</code>

### Made at:
<a href="https://hack36.com"> <img src="http://bit.ly/BuiltAtHack36" height=20px> </a>


## AI Proctoring
  
#### Concept:
<p>AI proctoring is the core of <code>AI PROCTORING MATE</code> Application. As the name suggests, It enables the possiblity of conducting examination,with proctors being Machine itself.</p>


#### Working:
<p>
It works as in, <b>As soon as the test starts at the student's end, the system's camera at the candidate's end starts capturing the video frames</b>. Upon this video frame, the <b>frontal_face_detector detects the count of faces in the frame</b>; blink detection script, evaluates if the <b>candidate is blinking (or ultimately looking down)</b> & the <b>Iris movements of the candidate is tracked , using gaze detection and face_detection_68_facial_landmarks data model</b>. Object Detection is also enabled in the test envoirnment.
</p>

<p>
  Via a <b>pre-tuned function</b>, this script considering <b>all the factors(blink, gaze, object detection, facial counts..)</b>, calculates a suspicion value, which is then compared with a Threshold value, and <b>if the suspicion value exceeds the threshold value; the student is given a warning( 2 times ), the 3rd time it happens, test ends automatically.</b>
</p>


## PART1 : UI Components:

<code>This is part 1 of <b>AI-PROCTORING-MATE</b> Application</code><br>
Use <code>&#x2713;</code> or <code>&#x2717;</code> for displaying Progress.

<strong>Description:</strong><br>

<p>This is the Candidate's end of the <code>AI PROCTORING MATE</code>.</p>

<p>
It comprises of the UI components for Setting up AI proctored envoirnment for the Quiz/test at the candidate's end.The UI has Sections (max. upto 3) depending upon the configurations set by the test creator.It has an in-built Calculator which is enabled according to the configurations instructions for the quiz given by the teacher.
Student gets the mark for review, unmark , reset response, select options for each question.
</p>

#### Working

<p>
  The first window in the UI is Get code which prompts the user to enter the test code.<br>
  The second window in the UI is the Get Details window which obtains the name and ID from the candidate.<br>
  Then the instruction menu is rendered for 90 seconds which shows basic test details like no. of sections etc.<br>
  The final window is the exam window which gets the responses from the candidate <br>
  Post completion of test(either thorugh timeout or submit test) a chrome automation is run which uploads the video and resposnse files pertaining to the test.
<p>

#### Proposed Features

1. Get Code Window
        
    - ✓   Prompts the candidate for the test code.
    - ✓   Checks the validity of the code.
    - ✓   Fetchs files of respective code.
    - ✓   Practice mode for people to get familiar.


2. Get Details Window

    - ✓   Prompts for the name and unique ID of the candidate.
    - ✓   Verifies if the ID format matches the one provided by the Teacher.


3. Show Information Window

    - ✓   Shows the candidate the information about the test like number of sections and if calculator is allowed.
    - ✓   Has a timer of 90 second which on lapse starts the test.


4. Main Exam Window

    - ✓ Renders the Questions dynamically
    - ✓ The question can be single or multi correct
    - ✓ Has buttons for each question for navigation directly to the question
    - ✓ These buttons change color depending on question status
    - ✓ Has next and previous buttons for navigation
    - ✓ Has 3 different sections with the ability to give different marking schemes for each section
    - ✓ Buttons at the top of UI to change section as well as the through next button of lest question
    - ✓ Has the option to bookmark question which displays a bookmark over the question button
    - ✓ Has timer at the top to show remaining time which turns red in the last 20% time
    - ✓ Has a calculator if the teacher allows one
    - ✓ Has the functionality to shuffle order of questions and options if desired
    - ✓ Closes automatically after one warning if application switch is detected after a warning
    - ✓ Records audio and video of the candidate
    - ✓ Displays a preview of the video being recorded
    - ✓ The video is processed by AI algorithms using parallel computation for speedup
    - ✓ Generates a ultrasound pulse and records its amplitude at regular intervals
    - ✓ Uploads the response file as well as video files of the candidate
    - ✓ Removes unnecessary files


  
  

## PART2 : Test Mate

<code>This is part 2 of <b>AI-PROCTORING-MATE</b> Application</code><br>
Use <code>&#x2713;</code> or <code>&#x2717;</code> for displaying Progress.

<strong>Description:</strong><br>
<p>
Test Mate is a web platform developed for easing the Burden of sophisticated Websites, on <b>online Test creators.</b><br> This website has authentication features like <b>User registration,Login and Logout</b>, with <b>Email-verification to Avtivate the account</b>, and <b>Reset password</b>, in case the user wants to do so.
</p>
<p>
  This Website consists of an interactive <b>User dashboard</b>, with Dynamic components like - <b>Stat cards</b> & <b>Response Summaries</b>. To give a brief to it's user, about his/her activity on the website, Test-Mate also provides a <b>dynamic Timeline</b>. 
</p>

  #### Purpose:
<p>
This Website as mentioned above, is biult for online Test Creators.It solves it's purpose by providing it's user, an Easy to <b>create Quiz</b>, with <b>dynamic Configuration setting</b>. User can <b>Schedule the quiz for a later date or time</b>. Moreover, he/she can <b>add upto 3 sections to the quiz</b>, and <b>can allot different number of questions in each section</b>. Apart from this, he/she <b>can also set positives & negatives per question for each section, in a particular quiz.</b>
Option for <b>Shuffling Questions and their options</b> for students end is also provided in the configuration. User can also choose, if we shall allow student to use <b>UI's in-built calulator</b> and <b>keep soft copy of the quiz questions, once the quiz is over</b>.
</p>
  
  #### Extra Features:

<p>
Once the quiz is created, he/she will be prompted to a webpage, with a <b>unique test code</b> for that quiz. which he/she can share with concerned students.
<b>UI of the Application will Auto download the quiz's test material</b> , once the student enters this test code at his end.If all the time validations(entering test code before scheduled quiz time, after scheduled quiz time), passes, the automation at the student's end will<b> auto submit his response</b>, and Any video/audio files created for that particular student to this websites, db.
</p>
<p>
 <b>Reponses received from the test(Quiz) will be evaluated, in the back-end</b>, and once the test is finished, the user, or test creator can see how well the students performed.Moreover, <b>he/she can download the recorded audio/video files of the student with links given corresponding to that particular event.</b>
 <b>Response summaries</b> will be <b>dynamically updated</b> and added, as soon as the teacher views the responses , on the user's Dashboard.
</p>  
<p>
  <b>Features for reaching students(feedbacks) and developers(in case of any discrepancies) via mailing service</b> is also provided on the website.
<p>

### Test Mate Progress

1. Home

    - ✓ Landing Page

2. Authentication

    - ✓ Registration
    - ✓ Login
    - ✓ Email Activation
    - ✓ Reset Password via Mail
    - ✓ Logout

3. Dashboard:
    
    - ✓ Create Dashboard
    - ✓ Create Quiz
        
        - ✓ Configurations Page
        - ✓ Dynamic Section's Page
        - ✓ Uniques Code Display Page

    - ✓ Stats Cards
    - ✓ Stats Plot
    - ✓ Activity Timeline
    - ✓ Quizzes Created
    - ✓ Responses Received

4. Feedback & Contact Us:
    
    - ✓ Reach Us Form
    - ✓ Feedback Form
