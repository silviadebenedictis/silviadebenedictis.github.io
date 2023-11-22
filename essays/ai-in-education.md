---
layout: essay
type: essay
title: "AI In Education: Where Do We Cross the Line?"
# All dates must be YYYY-MM-DD format!
date: 2023-11-21
published: true
labels:
  - AI
  - Software Engineering
  - Experiences
---

<img width="300px" class="rounded float-start pe-4" src="../img/smrt.png">

## I. Introduction
AI plays a significant role in both education and Software Engineering. Its purpose in education is to enhance learning by personalizing learning experiences and providing feedback to students. When it comes to software engineering education, AI is especially valuable during a developer’s coding process. AI-powered tools help out with detecting bugs, generating code and sample data, and also explaining the code.  One of these tools, which I’ve been using in ICS 314 during this semester, is ChatGPT. 

## II. Personal Experience with AI:
Prior to taking ICS 314, I’ve never used ChatGPT for code related questions, so I didn’t have high expectations of it until I first experimented with it in the class WODs.

### 1. Experience WODs 
I believe that the experience WODs already have clear instructions and videos, therefore ChatGPT is not needed for this element. I prefer practicing the WODs without using ChatGPT because it could result in overrelying on it, like using it for the simplest instructions.

### 2. In-class Practice WODs
I did not try using ChatGPT for in-class practice WODs because I felt that it defeats the purpose of learning through mistakes or taking your time to understand how to do the WOD without relying on AI. 

### 3. In-class WODs
One of the first WODs I used ChatGPT for was the “Surf Score”. When I wrote my code and tried running it, I had an error and couldn’t figure out what went wrong. I was running out of time and so I chose to ask ChatGPT:
```
Can you correct this code:
 class Score{
	constructor(judgeName, score){
  	this.judgeName = judgeName;
    this.score = score;
  }


}

class Ride{
	constructor(surferName){
  	this.surferName = surferName;
    this.scores = [];
  }
  addScore(score){
  	 this.scores.push(score);
  }
  printAllScores(){
  	for(let score of this.scores){
    	console.log('${score.judgeName} gave a score of ${score.score}');
    }
  }
```
And here is ChatGPT’s answer:
```
Certainly, I've noticed a couple of issues in your code. You need to use backticks (``) for string interpolation, and it should be ${score.judgeName} and ${score.score} inside the printAllScores() method. Here's the corrected code:
class Score {
  constructor(judgeName, score) {
    this.judgeName = judgeName;
    this.score = score;
  }
}


class Ride {
  constructor(surferName) {
    this.surferName = surferName;
    this.scores = [];
  }


  addScore(score) {
    this.scores.push(score);
  }


  printAllScores() {
    for (let score of this.scores) {
      console.log(`${score.judgeName} gave a score of ${score.score}`);
    }
  }
}
With these corrections, your code should work as expected.
```
It immediately found the issue, and returned my corrected code. While it’s true that we shouldn’t depend on AI for everything, I believe that in scenarios like this it’s very efficient to have a tool that provides quick feedback.

### 4. Essays
When it comes to writing essays, I try to avoid using AI tools because from past experiences I noticed that it always generated unnatural sounding essays. It chose complicated words that not even college students use and the sentences sounded stilted and robotic. I believe that AI algorithms are not yet advanced enough to write “human” essays.

### 5. Final project
So far I did not use AI for the final project pages because I did not think it was necessary. I’ve been applying what I’ve learned from other assignments and projects because they are very similar to the pages that our group has been working on. However, for future implementations, I believe that it will be useful to use when customizing the pages or accessing data from the collections. For instance, I could paste the code of my page along with the CSS file and ask ChatGPT how I can enhance the UI design. 

### 6. Learning a concept / tutorial
Although ChatGPT is useful in explaining a concept and showing a step by step tutorial, I feel more comfortable searching up the concept or watching a video related to it since I’m mostly a visual learner. Currently, ChatGPT does not provide features like images or videos so I don’t find it helpful for going through tutorials yet.

### 7.

### 8.

### 9.

### 10.

### 11.

## “Smart” Questions

So what makes questions “smart”? They are characterized by several key attributes, but the most important ones are that they are clear, concise, and specific. A good example of this is a question on Stack Overflow whose subject header is <a href="https://stackoverflow.com/questions/31453495/how-to-read-appsettings-values-from-a-json-file-in-asp-net-core">“How to read AppSettings values from a .json file in ASP.NET Core”</a>. The questioner starts off by showing how they set up their AppSettings data in a specific file.

```
I have set up my AppSettings data in file appsettings/Config .json like this:
{
  "AppSettings": {
        "token": "1234"
    }
}
```

They then mention how they searched the question online and could not find anything useful while also showing a snippet of what they tried to solve the problem:

```
var configuration = new Configuration();
var appSettings = configuration.Get("AppSettings"); // null
var token = configuration.Get("token"); // null

```

They conclude by asking how to specifically read their data from a .json file in ASP.NET Core:
```
I know with ASP.NET 4.0 you can do this:

System.Configuration.ConfigurationManager.AppSettings["token"];

But how do I do this in ASP.NET Core?

```

This question is considered 'smart' because it exhibits key attributes: clarity, conciseness, specificity, and a demonstration of prior research. The asker's effort to understand the topic and seek advanced information is evident.  As a result, several people gave answers that either provided a solution or explained the process of getting it.


##  “Not So Smart” Questions

Now that we’ve looked at what a “smart” question could look like, let’s see an example of the opposite of one. A user on Stack Overflow asks this:

```
How to change values in lower triangular of matrix in julia and transform to upper triangular? I need help with homework

```

There are no other details, examples or snippets of code included. The questioner clearly did not bother researching beforehand or trying their own code before getting an error, leaving the commenters confused. 

<img width="900px" src="../img/not-smart-q.png">

