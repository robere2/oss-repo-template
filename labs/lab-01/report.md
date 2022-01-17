# Lab 01 Report - Introduction to Open Source Software

## 1.

![Discord Message](Discord%20Message.png)

## 2.

### Smart Questions

* Sometimes, people realize they are working on a tech stack or with tools which are not appropriate for the job. As long as they realize this, you shouldn't push them to use something else. This can be out of their control.
* Extending off of point #2, when you link someone to a simple answer (such as a previously-answered question, FAQ, etc.), tell them how you found that resource. Many people do not realize these days how to properly use Google for tech searches.
* If you can't help someone and think someone might be able to find more help on another forum, for example, point them in the right direction.

### Free Culture
 
This is an interesting story. RPI still shares this story today at it's student orientation presentations (as of 2018), and paints Jesse in a bad light. They advertise him as a pirate which single-handedly ran a music distribution torrenting service across the entire internet. If this article is true, that doesn't appear to at all be the case. I understand RPI has liability it must protect, but lying (or at least misleading) to its students seems like a bad idea, given the current relations. I did a bit of research and fortunately it seems like it did not have a severely negative impact on Jesse's career. As of 2013 he landed a senior software developer position. It also showcases the frustrating part of America's civil legal system, which admittedly I don't fully understand. The fact that Jesse would reportedly not be able to receive back his $250,000 in legal fees if he were to win feels unfair. I know that this is not always the case, as I have seen news stories of people receiving back their legal fees. Perhaps this is done through a counter-suit? Regardless, this is a flaw that needs fixing, if it has not already been fixed.

## 3.

![man tree](Tree%20screenshot.png)

## 4.

![Regex Problem 1](Regex%20Problem%201.png)

![Regex Problem 2](Regex%20Problem%202.png)

![Regex Problem 3](Regex%20Problem%203.png)

![Regex Problem 4](Regex%20Problem%204.png)

![Regex Problem 5](Regex%20Problem%205.png)

![Regex Problem 6](Regex%20Problem%206.png)

![Regex Problem 7](Regex%20Problem%207.png)

![Regex Crossword 1](Regex%20Crossword%201.png)

![Regex Crossword 2](Regex%20Crossword%202.png)

![Regex Crossword 3](Regex%20Crossword%203.png)

![Regex Crossword 4](Regex%20Crossword%204.png)

![Regex Crossword 5](Regex%20Crossword%205.png)

## 5. Blockly

My first idea for the maze problem was to just continuously move forward until I reached a left turn, at which point turn left. This worked until I reached a point where I was forced to turn right. I had to add logic which checked three directions in the following order: left, then ahead, then right. Once it found a valid path, it moved that direction. This also worked until I reached a dead-end, at which point there are no valid paths in any of the three directions. I revised the code to make 2 right turns in the event of no right path, and this works, however I was able to make it slightly more efficient (uses one less block) by removing the double turn, and instead only moving forward if there is actually a path forward.

![Maze Solution](Maze%20Solution%202.png)

## 6.
https://github.com/vuetifyjs/vuetify
Vuetify is a library I've worked with extensively for my own projects but haven't contributed to personally. Despite this, I think I have a decent understanding of how the library functions internally (<`v3.0.0`), due to having to repeatedly refer to internal code to figure out how other components work. Vuetify has an extensive set of ready-to-use components for webpage design. I think it'd be really cool to design and implement my own component, with the hopes of eventually getting it added to the frameworks main set of components. This would probably be a difficult task, but at the very least, I would hope to get a proposal in and have it reviewed by the project lead(s).