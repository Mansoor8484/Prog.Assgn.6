# Prog.Assgn.6 Front End Quiz App

## Problem Statement

The Quiz app demo utilizes HTML, CSS and JS to collectively structure, style and logically provide a quiz like interface. The application will dictate how to go about completing the quiz, then provide the questions and correct answers upon answering each question. After completing the quiz, you can either quit or retake.

## Functional Features

- Start Quiz Button: Upon clicking "Start Quiz" you will be taken to the quiz directions.

- Quiz Rules: The quiz rules describe how to complete the quiz. Upon clicking "continue", you will be taken to the first question. If "exit quiz" is clicked then you will be taken back to the home screen.

- Questioning: You will be given 5questions, each with a 15 second timer. Upons cliking the answer, it will be verified as either right or wrong. The "Next Que" button will take you to the next question.

- After the last question is answered, you can click "Replay quiz" to take the quiz again or "Quit Quiz" to return to the home page.

## Codebase

The codebase is seperated into files isolating each language.

- The idex.html file is at root level in order for Pages to properly host the application.

- The JS folder contains all pertinent logical code for the questions themselves as well as the functions that manage the user input.

- The CSS file is responsible for styling all pages of the website.

- Note: the JS and CSS files are implemented in an external fashion, so the link and script tags are used to connect the external files to the index.html file.

## File Relevancy

- index.html: The index file is responsible for the content structuring of the website. iIt provides the content for each aspect of the website including the Quiz outline.

- quizApp.js: This file is responsibel for brining in all html elements and storing them as variables to be used for app functionality.

- questions.js: This file contains an array of js objects in which each onject has the attributes: numb, question, answer, and options (another array that has the options for the answers to the question).

  ### Functions in quizApp.js

  - showQuestions: Pulls data from the questions.js file and is responsible for showing the questions at each attribute

  - optionSelected: This functions is reaponsible fot checking what answer the user selected and determining it it was the correct one. It does so by using an if else statement to check if the users score should be increased or left alone. It also manages the disabling of selection after a answer is already sleected

  - showResult: This function will diaplay the total amount of answers corrctly answered by the user followed by a custom message based off of the score recieved

  - startTimer: Controls the timer and actions associated with it such  as srtting the interval, checking the time and  adding minute time details.

  - startTimerLine: Shows the progress bar in correlation to the time left on the clock.

  - queCounter: Counts the number of questions remaining

- style.css: Standard styling techniques used to style every aspect of the DOM. 


