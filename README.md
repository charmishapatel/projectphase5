# projectphase5


Project Phase 6



1.	What is your security recommendation? Why did you choose it?
I am using firebase inbuilt authentication for user login and signup. However, here rando email can be generated and logged in.
I can provide a link to create a profile through “google”, “github” etc to verify there are actual user at other applications.  

Since, I am using password, I need to give option for changing/forget password which should require re-authorization to ensure it is the actual user.

Secondly, the database I am currently using is public, which implies that anybody can read/write the data in firestore database. I need to learn to set up the condition for a read/write in database.


2.	Who does the recommendation benefit (end-user, developer, etc.)?
Adding a link to create profile through google will reduce the work for the user. As they are using the profile they created in google.
Re-authorization is utmost important to ensure that the user is the actual user. We can add security question and answer to verify.
For the database part, it is essential as the data can be changed without the permission of user. Basically, the whole data is open and is not protected.

3.	If the recommendation was found somewhere other than the provided checklist, include a link to it. 

I read the checklist and even researched online.
The point suggested above is common in both documents.
https://cheatsheetseries.owasp.org/cheatsheets/Mobile_Application_Security_Cheat_Sheet.html


4.	When would the recommendation have to be implemented (based on how serious the security risk is)?

I will change the read/write for database in this current week. I have already seen tutorial on it, and I felt it was easy as we just need to change rules into firebase.

For the re-authorization, I might work on it at the last after my whole application is built. I believe being new to react-native and firebase, re-authorization will be bit of a task to do and since I am not publishing this anywhere, I have 0 users.
Once the application is set up completely, I will start working on the password.


5.	Why do you think your project needs your recommendation?
The recommendation regarding the re-authorization is crucial for ensuring the security of the application. Without any re-authorization any fake profile can be created, and access can be gained to the application.  This can further change the user data inside the application. On top of that, such low-level secure application creates a sense of trustworthiness among user, which we do not want.

Similarly, open database allows anyone to change the data, it will even expose the user login credential. Changing the login credential will deny the access to actual user. 
Additionally, changing and data in the database will be reflected in the application and t

6.	How do you think your recommendation could be applied?

Firebases provide an option to authenticate user by logging in through google, GitHub etc.

7.	How feasible would the implementation be?

The implementation is highly feasible with Firebase's extensive support for security features and integration guides. However, I might take a little more time because I need to understand the concept thoroughly in order to implement it.
So far, I have tried it in web development and felt it was quite easy.

