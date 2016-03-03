# SavePlates
a save plate manager that works with google forms

My fraternity makes save plates for people who aren't able to come to lunch or dinner on any given day. We used to have a problem with people always requesting save plates on our groupme, but this created spam and wasn't always reliable because sometimes the people making saveplates wouldn't be able to find all the requests in the groupme. So I created this program to manage save plates for my fraternity. People are able to request save plates using the google form. If they want to sign up for a weekly save plate, then they can put a star next to their name. If there is no star next to their name, then the form will auto-clear their name after their save plate for that day has been made.

Submission is from a google form that can be viewed here
http://goo.gl/forms/W2FsJ3fGC5

There is a trigger that will run the function 'onFormSubmit' every time the form is submitted
That will populate the saveplates sheet using the submission that triggered the function
The sheet can be viewed here
https://docs.google.com/spreadsheets/d/1yGL8HWf9xyz_Bjde49bFy5hGo3YqC1FOgfkweKEjk0Q/edit?usp=sharing

Every day, save plates for dinner are made around 5:50. There is another triggered function 'clearNonStarsDay' that runs every day around 7pm that clears out the saveplate requests for that day. Non-starred names are deleted from the day, and starred names are collapsed to the top.
