---
layout: essay
type: essay
title: "Coding Standards"
# All dates must be YYYY-MM-DD format!
date: 2025-02-13
published: true
labels:
  - ESLint
  - VSCode
---



*Coding Standards*


## Introduction to ESLint
When I was working on ESLint for the first time, I went in without knowing what to expect, but one thing that I wasn’t prepared for was the time that it would take to set up. I ran into multiple errors while trying to do so, and the whole process took me about 30 minutes to fix, not including the time spent setting it up on VSCode.

When I tried following directions on the website from the FreeCodeCamp NVM installation guide for Macs, I copied and pasted the commands that were on the site step-by-step, like curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh bash and nvm -v, but source ~/.bashrc and nvm -v wouldn’t work no matter how many times I tried so I added export NVM_DIR= ... "$NVM_DIR/nvm.sh" to update my profile configuration, and when that didn't work, I tried reinstalling it by using curl ... install.sh again. I almost gave up because I kept getting an error message that said something along the lines of the terminal not being able to find the file or that it didn’t exist. Then somehow, when I messed around with some more things by randomly copying and pasting things I found on the internet in my terminal, I finally got it to work, but I don't know what it was that I did that made it work. I was just relieved to finally see the message showing me that NVM was installed successfully. Then, I moved on to trying to use it in VSCode when I thought I was finally done. However, I ran into even more issues because npm install wouldn’t work and setting up the packages were confusing as well. However, it all worked out somehow in the end.

<img width="350px" class="rounded float-start pe-4" src="../img/difficulty/allec-gomes-TWtnNL2MQCw-unsplash.jpg">

## Coding Standards
Intially, I couldn’t really get into using LSLint because I felt like the formatting that it wanted was trivial (e.g. spaces between curly brackets, no trailing spaces, new line required after ending of line of code) and the errors that it gave were too nit-picky. However, after I used it for some more time, I didn’t mind it as much anymore and started to keep the mistakes that I made in mind for formatting and fixed them to prevent getting errors beforehand. I understand why LSLint is important since it makes things more readable and neater, but I feel like if I was working on my own projects and I wasn't in a group setting, I would find it time-consuming to go through each line of code to meet its standards when I want to focus on other things instead, like implementation. However, I think it’s useful because it gives me confidence that I won’t run into any critical errors later on since it tracks down the errors beforehand and prevents parts of the code from clashing with other sections. Overall, I think LSLint is difficult to set up at first, but after getting used to running into errors and fixing the ones that LSLint points out, it's a great tool for productivity and improving the quality of code to meet coding standards.
