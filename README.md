# CTFs

This repository contains writeups of challenges designed by Hamza Haroon. 

Do not repost/copy any writeup or challenge without explicit permission of the author.

All Rights Reserved



# Emergency | OSINT | Hamza Haroon

## Hint: Time management is the key.

User is provided with an email:

`test.thegr1ffyn@gmail.com`

To get ahead with the question, we use [Epieos.com](http://Epieos.com) 

![Untitled](Emergency%20OSINT%20Hamza%20Haroon%2041577dbe5c1a49188af4cdd28f047045/Untitled.png)

We see that we can use this tool to perform OSINT on any email address. We search for our given email.

![Untitled](Emergency%20OSINT%20Hamza%20Haroon%2041577dbe5c1a49188af4cdd28f047045/Untitled%201.png)

We got this as a result:

![Untitled](Emergency%20OSINT%20Hamza%20Haroon%2041577dbe5c1a49188af4cdd28f047045/Untitled%202.png)

We are given a hint which tells us about how time management is very important to our user. Did you get it????? 

We see that we are given a Google Calender link that we can look into to find something juicy.

`https://calendar.google.com/calendar/u/0/embed?src=test.thegr1ffyn@gmail.com`

Ahhhh, here it is:

![Untitled](Emergency%20OSINT%20Hamza%20Haroon%2041577dbe5c1a49188af4cdd28f047045/Untitled%203.png)

So we have a hint:

**You are going in the right direction, continue perpendicular to the ground at SUM32768**

 **to find the emergency.**

Notice how we are given a string, we search it out on Google.

![Untitled](Emergency%20OSINT%20Hamza%20Haroon%2041577dbe5c1a49188af4cdd28f047045/Untitled%204.png)

Seems like the given string relates to some kind of flying as given in our hint as well. The first result is a tweet about an aircraft. Lets check:

![Untitled](Emergency%20OSINT%20Hamza%20Haroon%2041577dbe5c1a49188af4cdd28f047045/Untitled%205.png)

So this seems like the flight number of an aircraft that is being reported by a Twitter Investigator. We scroll down a bit to find another hint.

![Untitled](Emergency%20OSINT%20Hamza%20Haroon%2041577dbe5c1a49188af4cdd28f047045/Untitled%206.png)

Seems like we are almost there, all we need to do now is to find the time of landing and the total time of the flight on 7 February 2022. 

Flightradar24.com is a good tool to find information:

We enter the flight details:

![Untitled](Emergency%20OSINT%20Hamza%20Haroon%2041577dbe5c1a49188af4cdd28f047045/Untitled%207.png)

We check this to find the exact flying details on the specific date.

![Untitled](Emergency%20OSINT%20Hamza%20Haroon%2041577dbe5c1a49188af4cdd28f047045/Untitled%208.png)

So here we have our flag:

## `AOF{10:57PM_3:22}`

## Easter Egg:

Sometimes smart work is more efficient than hard work. If you went through the calendar, you will notice that one more memo is given on September 24, 2022.

Lets open it up:

![Untitled](Emergency%20OSINT%20Hamza%20Haroon%2041577dbe5c1a49188af4cdd28f047045/Untitled%209.png)

![Untitled](Emergency%20OSINT%20Hamza%20Haroon%2041577dbe5c1a49188af4cdd28f047045/Untitled%2010.png)

If we click on copy to my calender, it redirects to another page where we can see all the details of the memo. Notice how there is a file given in the attachments:

![Untitled](Emergency%20OSINT%20Hamza%20Haroon%2041577dbe5c1a49188af4cdd28f047045/Untitled%2011.png)

Lets open up the file:

![Untitled](Emergency%20OSINT%20Hamza%20Haroon%2041577dbe5c1a49188af4cdd28f047045/Untitled%2012.png)

ITS THE WHOLE ANSWER AHHAHAHAHA 🤣🤣🤣🤣🤣🤣🤣🤣🤣🤣🤣🤣

The whole question endpoint is given here. Its always better to look for more ways to find a clue. Hope it was fun to solve.
