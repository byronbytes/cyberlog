I have finally found a worthy reason to bypass the system. Look at this extension, that is actuvally a RAT (Remote Access Trojan) in disguise. In this journey, I will try to figure out how to bypass this.

![image](https://user-images.githubusercontent.com/53088136/135299328-f5cdc64e-7308-48a4-800a-18a50c681633.png)

Some very concerning things about this RAT is that it can view whatever you are doing at anytime, which is a massive invasion of privacy, I was also able to take a  at the site's "spy"board and was able to see that it can view what site you visit the most and what you are currently on. Of course, this site was most visited because I get bored and I like coding.

## Important Information
While taking a glance at the main panel, I have noticed that this has WAY more permission than it should have. It has the ability to see recent search history, capture the current screen (explained earlier in thread) and recordings (which I have no idea what that is). There is also a notification for "unusual browsing history" which will report searches, in an example I was able to see, it was "google snakw" (google snake).


Let's break down what permissions this unfairly inherits:

* Read and change all your data on the websites you visit

This means it can change what the website does, nothing special since most extensions have this.

* Capture content of your screen

This is a red flag. This means it can completely read and see what you are currently doing on your computer.

* Display notifications

Not as much of a red flag.

Another thing I noticed is that if I am currently in the middle of typing something, it cannot force close the site because there is unsaved work. After about 3 close attempts it does close, but this can be a start to something.


This also seems to be linked with an extension called Relay, which has equally high threats and privacy invasions, but worse.

Here is Relay:

![image](https://user-images.githubusercontent.com/53088136/135317700-3faf0c11-7f4a-46eb-a51e-f87a152a7a95.png)


Alright, this is way way worse and a much more severe RAT.



# Suspections
I suspect that RelayClassroom is for teachers monitoring the computers while in class, but the problem is that there is no pre-notification that you are being watched, and there is no way to know that you aren't being watched. So in theroy they could check up on you while you are in your HOUSE. Relay is most likely the main point and connector.


# The Drawing Board
So, we have now analyzed WHAT this is, HOW this is a problem and WHAT this problem can cause, now we have to figure out how to find a workaround for it.

## Idea #1 - Popup Creator
The first thing I noticed is that if the site gives a popup before closure, it will not close until it gets force-closed 2-3~ more times. We could code an extension that creates a pop-up on a whitelisted site closure.

### Pros
+ Will give an extra 30 seconds of reflex time.
+ Not annoying unless it was force-closed.

### Cons
- Not permanent.

## Roadblocks
![image](https://user-images.githubusercontent.com/53088136/135456604-4ae4bf90-1cdd-49c3-a9fc-cf9cda4b26f6.png)

Unable to create extensions. Well there goes that idea.

## Workarounds
You could try creating a website, and adding a popup spam, since basic HTML is the only thing needed for that. Unfortunately that cannot apply to every website, and only a select few, so I guess overall this cannot work.


## Idea #2 - Internet Connection (Success!)
While trying to find loopholes in the system, I have figured out that the extension is unable to access the device if it is not connected to the internet, this is very good news for us, as I was able to see the panel for me and it said "Loading". So I would say this is a current success.

### Pros
+ Complete bypass for anything
+ Leaves no trace
+ Does what it is supposed to do
+ Google Suite (docs, slides, etc) fully works offline.


### Cons
- You will have limited site access for as long it is disconnected
- Probably other stuff but I haven't tested it yet.
- Online Multiplayer stuff does not work

## Roadblocks
It still technically is "offline" which makes it tough to find out when to disconnect.

## Workarounds
I don't know, but I will research this more.


## Idea #3 (For Search History) - Redirect Spamming
They are also able to view your search history remotely, not really a problem but I guess finding out my coding stuff can lead to finding other stuff, so why not spam redirect it?

### Pros
+ Easy to make
+ Can work really well
+ You would need to scroll... a lot


### Cons
- If you actually use search history to get back to items, well sorry.
