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



While the heading of his question could be better, it does convey what he’s trying to figure out. Usually something as brief as “python date of previous month” is what other users would enter in as search terms on Google, making it easily found. Another good thing about the question is that it’s not just a question. The asker shows what he or she has done and that he or she has put in some effort to answer the question. And while it may not be as important as the question itself, the asker shows courtesy, which does increase the chance of getting an answer.

```
A: datetime and the datetime.timedelta classes are your friend.

1. find today
2. use that to find the first day of this month.
3. use timedelta to backup a single day, to the last day of the previous month.
4. print the YYYYMM string you're looking for.

Like this:

 >>> import datetime
 >>> today = datetime.date.today()
 >>> first = datetime.date(day=1, month=today.month, year=today.year)
 >>> lastMonth = first - datetime.timedelta(days=1)
 >>> print lastMonth.strftime("%Y%m")
 201202
 >>>

```
 
The asker received six possible answers, and he or she was successful in inciting discussion from multiple users. The answers themselves were clear and were devoid of the rumored sarcasm and hostility of “hackers.” Since I myself have referenced this page and found it useful, I can confidently say that it is a good question.

## The foolproof way to get ignored.

While there are decent questions that benefit everyone, there are those one can ask to create an entirely different effect. In the following example, a user asks how he would, in short, create a desktop application with Facebook.

```
Q: Facebook Desktop Notifier

I am a beginner programmer that have never used anything other than what's included in a language.

I am trying to create a desktop application that notifies me anytime I get an update onfacebook. 
How should go about doing this? Thanks in advance.

edit Sorry I was not clear. Is there any way to make a DESKTOP application with facebook?
```

A simple “yes” would have answered the question, but we know that’s not the sort of answer he or she is looking for. Fortunately, someone kindly responded with a link to Facebook’s developer website. The asker should have done more research on his or her potential project. Then further down the road, he or she could have asked more specific and detailed questions that wouldn’t require a thousand-paged response for a sufficient answer.

## Conclusion

When we rely on others’ generosity and expertise to provide answers to our questions, it should hold that the question we ask should be one that leads to efficient and effective help that not only benefits us, but also the people we ask and others who might ask the same question in the future. Thus, if you have a question… make it a smart one! Asking questions may not always get you the best answer, but asking them in a way that will make others want to answer them will increase the success of finding a good solution and make it a positive experience on all sides.
