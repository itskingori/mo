Code Review
===========

> Code review is systematic examination (often known as peer review) of computer
> source code. It is intended to find and fix mistakes overlooked in the initial
> development phase, improving both the overall quality of software and the
> developers' skills.
> ~ [Wikipedia][1]


Everyone
--------

* Accept that many programming decisions are opinions. Discuss tradeoffs, which 
  you prefer, and reach a resolution quickly.
* Ask questions; don't make demands. ("What do you think about naming this ...?")
* Ask for clarification. ("I didn't understand. Can you clarify?")
* Avoid selective ownership of code. ("mine", "not mine", "yours")
* Avoid using terms that could be seen as referring to personal traits. ("dumb",
  "stupid") Assume everyone is attractive, intelligent, and well-meaning.
* Be explicit. Remember people don't always understand your intentions online.
* Be humble. ("I'm not sure - let's look it up.")
* Don't use hyperbole. ("always", "never", "endlessly", "nothing")
* Don't use sarcasm.
* Keep it real. If emoji, animated gifs, or humor aren't you, don't force them. 
  If they are, use them with aplomb.
* Talk in person if there are too many "I didn't understand ..." or "Alternative 
  solution: ..." comments. Post a follow-up comment summarizing offline discussion.


Your code reviewed
------------------

* Be grateful for the reviewer's suggestions. ("Good call. I'll make that
  change.")
* Don't take it personally. The review is of the code, not you.
* Explain why the code exists. ("It's like that because of these reasons. Would
  it be more clear if I rename this class/file/method/variable?")
* Try to respond to every comment.


Reviewing code
--------------

Understand why the code is necessary (bug, user experience, refactoring). Then:

* Communicate which ideas you feel strongly about and those you don't.
* Identify ways to simplify the code while still solving the problem.
* If discussions turn too philosophical or academic, move the discussion offline
  to a regular Friday afternoon technique discussion. In the meantime, let the
  author make the final decision on alternative implementations.
* Offer alternative implementations, but assume the author already considered
  them. ("What do you think about using a custom validator here?")
* Seek to understand the author's perspective.


[1]: http://en.wikipedia.org/wiki/Code_review
