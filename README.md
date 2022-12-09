# CS-499-Category-1-Software-Desgin-and-Engineering


The artifact: Inventory App
Inventory app was first created in CS-360 Mobile Architecture and Programming class. 
For my enhaced inventory app, I was supposed to have a login screen and an inventory activity responsible for collecting and viewing data.
When I was done with my login activity for the inventory app, I felt proud of the work that I had performed and in 
the appearance of the app. The app ran smoothly from login activity to the inventory activity. The .xml file had a 
lot of creative features that I had added ranging from text size, font, color, sheer background image more.

My inventory app was rather simple for my CS-360 class. I had first started with creating a login activity which was not connected to any 
database. The login was simple username: Admin and the password: admin. As the class proceeded, I learned to incorporate a database into 
the app, to which then I added a firebase database for better functionality of the app. At the time of submission, the login activity was
a success, and I had a RegisterActivity, which was also a success. While reworking on this Inventory app, I found a bug in the login and 
registration activities. Therefore I started from scratch for my submission in CS-499. The bug: when the user was successfully registered 
into the firebase database but the app would prompt the message “registration failed. Try again”. I worked a day or two to try to fix the
bug. Since the problem did not get fixed, I went ahead and created another inventory app. This helped me save time. In just half a day I 
had a great login activity, register activity, google login feature and finally the inventory app’s main screen. Now the login activity 
and the registration are properly linked into the firebase database. The app successfully allows registration and login to be prompted to 
the next screen, InventoryActivity. 

For my enhancement Plan I had wanted to create a feature that would allow the user to login via Google credentials. Once the user is prompted 
to the Inventory Activity, the user can click to add product, delete product, view inventory, or update inventory. All these features add, 
delete, view, and update are still in progress since I have to incorporate them into the Category 3: Database artifact enhancements. Yes, I 
have met the enhacement plan. I have added a google login feature, and recreated the main inventory screen with add, delete, view and update 
inventory buttons.
There were two challenges that I faced when recreating the inventory app. Challenge One: creating a dynamic link in firebase. It had got 
rather tough for me to find the SHA-1 fingerprint. SHA-1 is a unique key generated for the PC that can be used for signing. When creating
google sign in feature, I had to submit the SHA-1 keys for using the Google APIs. I then found the SHA-1 key using the gradle feature in 
the android studio. Challenge two: When I tried to login, even if it was successful, the app would crash. I researched a lot to find out 
why the app is not getting directed to next page, InventroyActivity, after successful login. After staring at the code for what felt like 
forever,  I realized that I had not created the method findViewById. I added the method, and the problems was fixed. Now the app is 
successfully performing the tasks it is supposed to.


LoginActivity: responsible to login the user and direct the user to the main InventoryActivity
RegisterActivity: responsible to register the user and directed back to the login screen. RegisterActivity screen is opened when the user 
clicks, create an account? The RegisterActivity also allows the user to be directed to the login screen when the user clicks, already have
an account?
The added feature on the Login screen is the Google sign in activity. In this activity, when the user clicks the Google icon on the login screen,
the app redirects the user to login via google credentials.
InventoryActivity: Once the user is successfully logged in, the user is directed to the InventoryActivity screen. On this screen, the user is
presented with 4 options: add product, delete product, view product, and update product. Each of these options are a button, when the user 
clicks add product, the user is directed to the AddActivity, and so on. 
Each of these (add, delete, view and update) options will be enhanced in the category 3 milestone: database. 

