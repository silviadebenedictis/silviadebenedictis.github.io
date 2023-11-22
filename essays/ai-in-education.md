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

<img width="400px" class="rounded float-start pe-4" src="../img/ai-image.jpg">

## I. Introduction
AI plays a significant role in both education and Software Engineering. Its purpose in education is to enhance learning by personalizing learning experiences and providing feedback to students. When it comes to software engineering education, AI is especially valuable during a developer’s coding process. AI-powered tools help out with detecting bugs, generating code and sample data, and also explaining the code.  One of these tools, which I’ve been using in ICS 314 during this semester, is ChatGPT. 

## II. Personal Experience with AI:
Prior to taking ICS 314, I’ve never used ChatGPT for code related questions, so I didn’t have high expectations of it until I first experimented with it in the class WODs.

#### 1. Experience WODs 
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

### 7. Answering a question in class or in Discord
I only answer questions that I’m confident in or when I had the same question that I found the answer to. Looking it up on ChatGPT could have helped answer the student’s question, but because not every information provided by it is correct, I would rather not risk spreading it. 

### 8. Asking or answering a smart-question
Similar to my previous response, I would not answer a smart question unless I’m very familiar with the topic, so even if ChatGPT could have, if I don't know how to explain it in my own words or am unsure if it's correct, I cannot use AI to answer someone's question. If I have a smart-question related to the class, I would ask it either in class or Discord.

### 9. Coding example
I did not ask ChatGPT for coding examples because I preferred searching for examples on from google or documentation sites. I enjoy “researching” examples instead of getting a straightforward answer because I get to learn more through error and trial.

### 10. xplaining code
I did not ask ChatGPT to explain code because most of the codes for ICS 314 already had documentation or an explanation from the assignment instructions.

### 11. Writing code
An example of when I asked ChatGPT to write code for me is when I was reimplementing my Bootstrap 5 <a href="https://courses.ics.hawaii.edu/ics314f23/morea/react/experience-yourchoice-react.html">“Your Choice”</a> mockup using React. Because the code is too lengthy to show I will summarize how my experience went with ChatGPT. I asked ChatGPT to “reimplement my mockup to use React”, and it immediately converted it to use React, following a similar process for the as the Island Snow React reimplementation from class. The only parts that I had to edit myself were the positions of the texts, icons, and images of my mockup. Therefore, I think AI is extremely useful for writing code, and although it comes with some flaws, it saves a lot of time to write the layout and debug the code.

### 12. Documenting code
My previous example applies to this as well. ChatGPT wrote my code along with helpful documentation, especially for lines of code that I wasn’t familiar with. 

### 13. Quality assurance
My example of the “Surf Score” issue applies here too. 

### 14. Other uses in ICS 314 not listed
Although I mentioned that AI is not useful for writing essays, I did use ChatGPT to come up with essay titles when I felt that I lacked the creativity for it. It provided me with multiple titles, and even though some examples sounded lengthy and boring, I was able to use AI as a way to come up with titles.
For example, for E28 I copied my essay about coding standards over to ChatGPT and asked:

```
What would be a fun and interesting title for the following essay : <a href="https://silviadebenedictis.github.io/essays/coding-standards.html">(my essay)</a>
```
ChatGPT’s answer: 
```
"The Code Chronicles: Navigating the Maze of Coding Standards for Efficient and Error-Free Programming"
```
My response: 
```
Give me another title but make it shorter
```
ChatGPT:
```
“Coding Standards: The Rules to Rule Code”
```
For other essay titles, it took several tries of asking for a better title until I found one I liked. I then realized that I needed to be more specific in what I wanted, which got the job done.

## III. Impact on Learning and Understanding:
The incorporation of AI in my software engineering course, particularly through the use of ChatGPT, has had a notable impact on my learning experience. One significant aspect is the enhancement of comprehension. When facing coding challenges or errors, ChatGPT provided quick and accurate feedback, facilitating a deeper understanding of the code. Like the "Surf Score" WOD example, ChatGPT swiftly identified errors and offered a corrected code, helping not only in problem resolution but also in understanding the mistakes I made. Additionally, AI has played a role in skill development. Utilizing ChatGPT to generate code examples, especially during the implementation of my Bootstrap 5 mockup using React, accelerated the coding process. However, because I had to adjust some elements manually, I felt that I was also learning how to read and personally customize the code to meet my expectations.

## IV. Practical Applications:
Outside of the classroom, AI has many practical applications in real-world software engineering projects. While my experience in ICS 314 focused on educational aspects, AI has been widely employed in industry settings. For instance, in the Hawaii Annual Code Challenge (HACC), the Lahaina Digital Twin Project used AI to contribute to data analysis. Its ability to process vast amounts of data and identify patterns makes it a valuable tool for addressing real-world software engineering challenges.

## V. Challenges and Opportunities:
While the integration of AI in class has been generally positive, I encountered certain challenges. One limitation is the dependency on AI for tasks that could hinder individual learning. For example, relying too heavily on ChatGPT for code corrections during WODs might discourage the development of independent problem-solving skills. Balancing the use of AI as a tool for assistance rather than a crutch is crucial to overcoming this challenge.
A potential opportunity for further integration of AI in software engineering education lies in customizing pages and accessing data in real-world projects. For instance, utilizing ChatGPT to enhance UI design or seeking advice on code optimization could be valuable in creating more robust and user-friendly software.

## VI. Comparative Analysis:
In comparing traditional teaching methods with AI-enhanced approaches in software engineering education, I believe engagement is one area where AI can offer a more interactive and immediate experience. ChatGPT's ability to provide instant feedback fosters engagement by addressing questions in real-time, which may not be achievable in a traditional classroom setting. Students also have the chance to ask an unlimited amount of questions without worrying about being criticized or made fun of for lacking knowledge. Furthermore, while traditional teaching methods rely on lectures, readings, and hands-on practice, AI supplements these approaches by offering personalized learning experiences. The quick feedback and assistance provided by ChatGPT contributes to a more dynamic and adaptive learning process, potentially improving knowledge retention.

## VII. Future Considerations:
Looking ahead, the future role of AI in software engineering education holds both promise and challenges. Advancements in AI capabilities, including incorporating visual and interactive elements in AI-driven educational tools could cater to diverse learning styles, benefiting visual learners like myself. Furthemore, as AI tools are fed more data over time, they will be more efficient in helping students with large coding projects. At the same time, the problem of overreliance will persist. If students get an immediate answer to a coding assignment without putting any effort into it, they will have learned nothing. To prevent this issue, it's important to keep a balance between traditional teaching methods and AI-enhanced approaches.

## VIII. Conclusion:
In conclusion, the integration of AI, particularly ChatGPT, in my software engineering course has positively influenced my learning journey. It has enhanced comprehension, accelerated skill development, and provided valuable assistance in problem-solving. The practical applications of AI extend beyond the classroom, offering innovative solutions to real-world software engineering challenges.
Despite challenges such as accuracy and the risk of overreliance, the future of AI in software engineering education looks promising. One suggestion I have for optimizing the integration of AI in future courses is to implement a structured and gradual approach to AI usage. Instead of introducing AI tools abruptly, educators can design a curriculum that progressively incorporates AI at various stages of the course. This allows students to build a strong foundation in traditional problem-solving and coding skills before relying on AI assistance.

