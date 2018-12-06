# AntiSpamAutomation
Using selenium module for python and chrome/gecko driver for form automation and spamming the scammer's database

NOTE: The following website is down apparently 

A few days ago http://pay.tm-cash-offers.in this link was sent to me via WhatsApp. Obviously this is not the genuine site and quite mallicious. This site was taking data (Name and mobile number) with a promise to reward 1000 Rupees to whoever answers 4 simple questions. Now Obviously the questions were only for show and one could easily bypass the 4 quesions stage of the website. Later the site demands to share the link of this website to 20 more friends on WhatsApp to collect the money. Now Even after clicking more than 100 times there was no signs of truth in their words.

That's why I thought, what if I could stop them. 

I created a simple python program with selenium that automates the data sending process and spamms their server with real looking 'fake' data.

I gathered some random names and surnames and put them inside a list. Now I live in India so I gathered some Indian names.

Generated random indices of the list and appended them in a string.

Generated random phone numbers starting with 9 ( as most Indian numbers start with 9)

Opened the link and fetched elements where data could be entered. This could be done in many ways. One common way is openeing the chrome console or other debugger console of your browser and then find the element by XPATH. Other ways could be finding the element by using name or tag. It really depends what you could find at the moment.

Then at this fetched position, enter the data by send_keys() function.

Go back to the starting link

By doing the above mentioned tasks in a loop we have succesfully started spamming the server.


Q. How it is actually helping?

A. By sending real looking data to the scammers, we actually make them think the data is real and they have no way other than calling the individual phone numbers to verify the genuinity. Meanwhile if a genuine guy guy enters data during the process of spamming, the real data gets sandwitched inside thousands of fake data. So there is no other way other than calling and verifying each individual phone number. This wastes the time of scammer. 

Q. How this can be imporved ?

A. By making a long list of names and surnames, by generating more authentic phone numbers by setting the first few digits in  a pre defined way (according to the telecom operators) i.e setting first four digits as "9836"(vodafone india) then the rest 6 digits are set randomly.

P.S NOTE: THE WEBSITE IS CURRENTLY DOWN. THE UPLOADED CODE DOESN'T WORK ANYMORE HOWEVER, THERE ARE CURRENTLY MANY MORE SCAMMY WEBSITES. SETTING YOUR OWN XPATH AND FIND BY ID WITH NEW LINK YOU COULD EFFICTIVELY DO THE SAME THING.

OR EVEN BETTER.

ANY CHANGE IS WELCOME TO MAKE THE CODE BETTER.
