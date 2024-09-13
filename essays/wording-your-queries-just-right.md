---
layout: essay
type: essay
title: "Wording Your Queries Just Right"
# All dates must be YYYY-MM-DD format!
date: 2024-09-12
published: true
labels:
  - StackOverflow
---

<img class="img-fluid" src="../img/smart-questions/smart-questions-header.png">

# The Importance of Asking the Smart Way

It’s common to get stuck on a problem in your code, causing you to spend hours troubleshooting, reading up on documentation, and trying out every combination of arguments and functions you could think of. Eventually, you might let go of your pride and express your question for the whole world to see. StackOverflow is the platform made for this, and receiving the kind of answer you want can require a lot of forethought and planning. This is why Smart questions are so valuable in these spaces. By following just a few simple rules, the quality of a question can dramatically improve, and the responses that follow can be more than helpful. As stated in the essay by Eric Steven Raymond:

> “We're not asking you to genuflect to us — in fact, most of us would love nothing more than to deal with you as an equal and welcome you into our culture, if you put in the effort required to make that possible.”

The key ingredient here is the effort you put into your question and the attitude you present to the people trying to help you. If you’re not willing to help yourself, or actively search for a solution, the volunteers on these forums may be less willing to assist you.

# How Should I Ask?

Before even writing the title of your question, there are a few key things that Raymond suggests you do:

1.Try to find an answer by searching the forum
   - Or the web
   - Or reading the manual
   - Or reading an FAQ
   - Or asking a skilled friend
   - Or through experimentation
   - Or by reading the source code

Way before even typing the question, someone else on the Internet might’ve had the same problem as you. Simply querying the problem on the web can bring you a myriad of solutions where people ran into the same issue. Additionally, by Googling, you can be brought to documentation that illustrates fixes to common problems. But once you have exhausted all sources and cannot locate solutions, then consulting a forum might be your best bet.

# The Smart Way

To show a question being asked the right way, I was able to locate this deceptively simple question:

[“What is the '-->' operator in C/C++?”](https://stackoverflow.com/questions/1642028/what-is-the-operator-in-c-c)

When I first found this question, I was a little confused about what the author was asking. My first thought was that they were questioning what the arrow operator was in C/C++, commonly written as “->”. This is a very trivial question and it’s probably one of the first things brought up in a C course when the instructor goes over pointers and structs. However, looking deeper into the question, there were two dashes, indicating that it wasn’t a normal arrow operation. Eventually, the repliers were able to answer the question, stating that it was a combination of operators, more specifically the decrement (--) and greater than (>) operator.

In my opinion, this question was pretty smart. Even though the question and answer were very straightforward, it was something that I couldn’t find information on. When I googled “--> operator”, the results I found (other than that StackOverflow question) were tutorials and articles written on the arrow operation (->). The question wasn’t easily Googleable, which probably made the author even more confused. Additionally, the author was smart in how they worded the question. The author put an example of the code and its output, which allowed for an easy understanding of what the code was meant to do. The title was also concise and descriptive. Instead of simply writing “what is this” in the title, he put the operator and defined the language. Everything was grammatically correct, and the answer was simple and concise.

# The Unsmart Way

On the other hand, there are a handful of questions on StackOverflow that are less than stellar. For example, this question:

[“is there a way i can fix this?](https://stackoverflow.com/questions/78980081/is-there-a-way-i-can-fix-this)

In addition to the vague title, the author simply put the stack trace and code block in the description. There are no words to describe the problem, no examples, and no intended output. It’s just a mess of code with no great leads on how to even begin to solve the problem. In addition, the post was marked as a duplicate, indicating that the question was asked before. The author didn’t even consider Googling the problem to see if other people had the same issue. Fortunately, someone in the comments echoed the same sentiment:

> “And in future, google your error message before posting a question...it's very rare that you're the first or only person to experience any given message.”

This is a terrible way to ask a question and it doesn’t follow any Smart rule listed in the essay.

# In Conclusion...

The importance of using the Smart structure to write a clear question cannot be understated. This structure helps developers get their point across more clearly and it can be helpful in the long run for people who run into the same problems. All in all, I learned a lot on how to write a well-structured question and I hope to apply it in the future when I hit a wall with my code.