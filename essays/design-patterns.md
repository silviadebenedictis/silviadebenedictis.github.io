---
layout: essay
type: essay
title: "Design Patterns: Tailoring Code with Threads of Wisdom"
# All dates must be YYYY-MM-DD format!
date: 2023-11-30
published: false
labels:
  - Design Patterns
  - Software Engineering
---

<img width="600px" class="rounded float-start pe-4" src="../img/design-pattern.png">

## Design Patterns

In the world of software developing, design patterns serve as the finely woven threads that stitch together the fabric of efficient, maintainable, and scalable code. Just like a skilled tailor who selects patterns to craft a custom suit, programmers must also choose design patterns that perfectly fit the contours of their problem domain. So, what exactly are some of these design patterns, and how have they elegantly adorned the garments of my code?

## The Patterns to My Problems

Imagine the software universe as a grand wardrobe, where each pattern represents a unique style statement. At the heart of this wardrobe lies the Factory pattern, akin to a master tailor setting up an assembly line to produce garments with precision and efficiency. In one of my coding assignments, I had to create an animal kingdom that could take in a variety of animals. The first version of my code could only handle information about dogs, so the bulk of my code lived inside the ‘Dog’ class, creating a structure that lacked flexibility. Because of this I needed a more versatile approach, which is where the Factory pattern came into play. Just as a tailor crafts various suits from the same template, I used the Factory pattern to instantiate different Animal subclasses, each with its specialized characteristics. This not only enhanced code readability but also facilitated easy extension when introducing new members to the animal family.

Now picture a bustling fashion show, where models and designers stay in sync without directly communicating. This synergy mirrors the Observer pattern, where objects—like models on a runway—notify and update their dependents just like designers awaiting the latest trend. For instance, in one of my ICS courses, I had to build a mobile app using Flutter. Most Flutter apps, being dynamic and event-driven, demand real-time updates, and my app required a method that would notify multiple widgets because of the changes being made to the pages. The solution I found to this was the Observer pattern, an invaluable asset that improved my app’s functionality. Through this pattern, widgets subscribe to changes in the application state, ensuring that the user interface seamlessly adapts to evolving data. It's like a well-coordinated fashion show where every piece of fabric aligns with the pulse of the event.


## Conclusion

In conclusion, the world of software development is not merely about writing lines of code but crafting a strategy of patterns that enhance the code. Just like tailors, programmers also weave the threads of design patterns into a codebase that stands the test of time. So, the next time you're asked about design patterns, think of them as the wardrobe essentials that elevate your code from mundane and problematic to exceptional and smooth, and let the stitching of wisdom continue. Happy coding!

