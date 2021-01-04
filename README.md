# tasked
Task management/monitoring library just made easy as builtin logging.

# caveat

In this asynchronous paradigm, more and more of the programs we handle becomes faster, but at the same time, complicated. We are having much more trouble tracking which programs/tasks are done and what are not then a single main() function that we only needed to think about.
When we first got the idea of separating modules, someone also came up with a brillient idea of logging and log-managers. With log-managers, we were able to concentrate on our programs and throw everything into the manager and let it do the dirty work.
This is the momement where we got the abillity to track down events chronologically when executing programs, and it was a major breakthrough to make bigger programs and libraries get there hang on what they're doing. 
But there was a subtle implication here if we wanted to know what is going on now.
When we look at a log of a traditional system or a program, if we wanted to know what it's doing right now, we only needed to focus on the very bottom, since what was going on will appear one by one at the bottom and most likely the adjascent (or nearby) logs are somewhat related and you could probably guess what the program was executing now.
But now after gradually shifting towards the era of asynchronousness, the implecation also changed, and it became harder and harder to know what is going on in a program at a point.

This is where the idea of task management/monitoring comes in. Like logs, tasks occur in many places of a program. Maybe one of them finishes faster than another, or it may consume more machine power and be slower. When we try to track these with just logs, it's becoming more and more of a pain. 

It is nothing new or something that people missed, but I think it's something people didn't catch the full potential of. It is more than a problem of local implementation, but a 
