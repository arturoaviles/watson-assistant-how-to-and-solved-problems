# Two Intents With Big Confidence - THE GREETING PROBLEM

##Problem:

Having 2 or more intents (Ex. #Greeting #Buy, etc.) and receiving a text from the user in which both intents have high confidence.

###Example:

Hello good afternoon, I want coffee

##Solutions:

### Solution 1 (Sometimes not the best one):

One option is to ask the user what it really meant.

####Example:

What did you want to say?

_Hello_
_Buy Something_

### Solution 2 (What if #Greeting is not that important)

We can transform __#Greeting__ to __@Gretting (Intent to Entity)__

This way, even when the user says:

"Hello good afternoon, I have a question, I want coffee."

Watson Assistant will send you to the #Buy Intent.*

*__It's important to mention__ that you need to put the __dialog node__ which recognizes __@greeting__ after all the intent dialog nodes.



