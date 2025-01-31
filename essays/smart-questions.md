---
layout: essay
type: essay
title: "Smart Questions, Good Answers"
# All dates must be YYYY-MM-DD format!
date: 2025-01-25
published: true
labels:
  - Questions
  - Answers
  - StackOverflow
---

<img width="300px" class="rounded float-start pe-4" src="../img/smart-questions/rtfm.png">

## Smart Questions

There are different ways to define a smart question, but the most common way to tell that it's smart is that it's noticeably a question that the original poster has attempted to find the answer themselves first through their own means, and if they can't find them, then their question posted on Stack Overflow should be formatted in a way that shows that they've already researched how to answer the question themselves but might need more clarification. For example, they might provide their own code that has issues that they can't resolve but shows that they've attempted it themselves beforehand. Another obvious sign that it's smart is if it's not outright asking for homework answers and such since asking those types of questions isn't meaningful and doesn't help the person who asked or other people who might see the post learn. 

An example of a good question is this:
```
I've recently spent a significant amount of time debugging a problem with a string inside my code.

This produced an error:

"root:password@tcp(127.0.0.1:3306)/employees?readTimeout=15m‌​"
This worked fine:

"root:password@tcp(127.0.0.1:3306)/employees?readTimeout=15m"
As you can see the strings look exactly the same, but when printed out in binary format:

First string:
[114 111 111 116 58 112 97 115 115 119 111 114 100 64 116 99 112 40 49 50 55 46 48 46 48 46 49 58 51 51 48 54 41 47 101 109 112 108 111 121 101 101 115 63 114 101 97 100 84 105 109 101 111 117 116 61 49 53 109]

Second string:
[114 111 111 116 58 112 97 115 115 119 111 114 100 64 116 99 112 40 49 50 55 46 48 46 48 46 49 58 51 51 48 54 41 47 101 109 112 108 111 121 101 101 115 63 114 101 97 100 84 105 109 101 111 117 116 61 49 53 109 226 128 140 226 128 139]

The second string happens to have extra two invisible Unicode characters at the end 226 128 140 226 128 139 that represent ZERO WIDTH NON-JOINER and ZERO WIDTH SPACE.

As it turns out, Stack Overflow inserts invisible characters inside long code comments.

When writing a comment like this:
aaaaaaaaaaaaaaaaaaaa‌​aaaaaaaaaaaaaaaaaaaa‌​aaaaaaaaaaaaaaaaaaaa‌​aaaaaaaaaaaaaaaaaaaa‌

My question is, why does Stack Overflow do this?

Why is inserting invisible characters into code snippets and effectively creating debugging nightmares considered a good solution?
```

The way that the author formatted this question shows that they have already taken time to understand what their problem is and attempted to resolve it on their own. Then, they gave snippets of their code, as well as the errors, and asked a valid question to better understand why they ran into their issue. This is also a potential question that other people might have, so it's helpful for others to reference from in the future.

On the contrary, there are bad questions.

## Not Smart Questions

An example of a not-so-smart question is this: 

```
What is the Perl equivalent of Python's time.time(), which returns the system time in fractional seconds?
```
That was the only sentence written in the question, with no other context or code provided. This is a poorly written question because the answer can be easily found online if the author simply looked for it. These types of questions are "bad" because it's not worth answering and isn't meaningful in any way that would help other people.

## Conclusion
It may be tempting to ask questions on Stack Overflow and expect a solution immediately, but before asking, it's best to think about whether it's smart or not. People should first think of whether it's a question that has been asked before, and if the solutions are already provided online. 
