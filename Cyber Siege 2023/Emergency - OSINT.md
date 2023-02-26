# Emergency | OSINT | Hamza Haroon

## Hint: Time management is the key.

User is provided with an email:

`test.thegr1ffyn@gmail.com`

To get ahead with the question, we use [Epieos.com](http://Epieos.com) 

![image](https://user-images.githubusercontent.com/95119705/221402085-3f4e4ee3-6691-4038-a81d-c6f51e47a702.png)


We see that we can use this tool to perform OSINT on any email address. We search for our given email.

![image](https://user-images.githubusercontent.com/95119705/221402116-ec64239d-c0e0-49f4-80f5-0038a2bedabe.png)


We got this as a result:

![image](https://user-images.githubusercontent.com/95119705/221402129-89d7f6f7-3a82-472e-838b-5f7cd85968b5.png)

We are given a hint which tells us about how time management is very important to our user. Did you get it????? 

We see that we are given a Google Calender link that we can look into to find something juicy.

`https://calendar.google.com/calendar/u/0/embed?src=test.thegr1ffyn@gmail.com`

Ahhhh, here it is:

![image](https://user-images.githubusercontent.com/95119705/221402140-c9efa949-d96f-42a9-a64a-8031b0454b8b.png)

So we have a hint:

**You are going in the right direction, continue perpendicular to the ground at SUM32768**

 **to find the emergency.**

Notice how we are given a string, we search it out on Google.

![image](https://user-images.githubusercontent.com/95119705/221402205-a84cc8b9-0848-4731-b2bd-dca349ee4111.png)

Seems like the given string relates to some kind of flying as given in our hint as well. The first result is a tweet about an aircraft. Lets check:

![image](https://user-images.githubusercontent.com/95119705/221402210-a945d1eb-1b08-4cd2-83e6-81b292bef948.png)

So this seems like the flight number of an aircraft that is being reported by a Twitter Investigator. We scroll down a bit to find another hint.

![image](https://user-images.githubusercontent.com/95119705/221402227-98f93add-662c-4ab8-ba8f-7ae91d655782.png)

Seems like we are almost there, all we need to do now is to find the time of landing and the total time of the flight on 7 February 2022. 

Flightradar24.com is a good tool to find information:

We enter the flight details:

![image](https://user-images.githubusercontent.com/95119705/221402258-17cb41e4-79ac-4dea-8118-5f2a92e067ba.png)

We check this to find the exact flying details on the specific date.

![image](https://user-images.githubusercontent.com/95119705/221402248-64df8a9e-e08e-4be8-80eb-95bde34cb136.png)

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
