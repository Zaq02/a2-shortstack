Assignment 2 - Short Stack: Basic Two-tier Web Application using HTML/CSS/JS and Node.js  
===

Due: September 8th, by 11:59 AM.



Deliverables
---

Do the following to complete this assignment and acheive a base grade of 85%:

1. Fork the starting project code (make sure to fork the 2022 repo!). This repo contains some starter code that may be used or discarded as needed.
2. Implement your project with the above requirements.
3. Test your project to make sure that when someone goes to your main page, it displays correctly.
4. Deploy your project to Glitch, and fill in the appropriate fields in your package.json file.
5. Ensure that your project has the proper naming scheme `a2-yourGithubUsername` so we can find it.
6. Modify the README to the specifications below, and delete all of the instructions originally found in this README.
7. Create and submit a Pull Request to the original repo. Label the pull request as follows: a2-gitusername-firstname-lastname

Acheivements
---

Below are suggested technical and design achievements. You can use these to help boost your grade up to an A and customize the assignment to your personal interests. These are recommended acheivements, but feel free to create/implement your own... just make sure you thoroughly describe what you did in your README and why it was challenging. ALL ACHIEVEMENTS MUST BE DESCRIBED IN YOUR README IN ORDER TO GET CREDIT FOR THEM.

*Technical*
- (10 points) Create a single-page app that both provides a form for users to submit data and always shows the current state of the server-side data. To put it another way, when the user submits data, the server should respond sending back the updated data (including the derived field calculated on the server) and the client should then update its data display.

*Design/UX*
- (5 points per person, with a max of 10 points) Test your user interface with other students in the class. Define a specific task for them to complete (ideally something short that takes <10 minutes), and then use the [think-aloud protocol](https://en.wikipedia.org/wiki/Think_aloud_protocol) to obtain feedback on your design (talk-aloud is also find). Important considerations when designing your study:

1. Make sure you start the study by clearly stating the task that you expect your user to accomplish.
2. You shouldn't provide any verbal instructions on how to use your interface / accomplish the task you give them. Make sure that your interface is clear enough that users can figure it out without any instruction, or provide text instructions from within the interface itself. 
3. If users get stuck to the point where they give up, you can then provde instruction so that the study can continue, but make sure to discuss this in your README. You won't lose any points for this... all feedback is good feedback!

You'll need to use sometype of collaborative software that will enable you both to see the test subject's screen and listen to their voice as they describe their thoughts. After completing each study, briefly (one to two sentences for each question) address the following in your README:

1. Provide the last name of each student you conduct the evaluation with.
2. What problems did the user have with your design?
3. What comments did they make that surprised you?
4. What would you change about the interface based on their feedback?

*You do not need to actually make changes based on their feedback*. This acheivement is designed to help gain experience testing user interfaces. If you run two user studies, you should answer two sets of questions. 

Sample Readme (delete the above when you're ready to submit, and modify the below so with your links and descriptions)
---


## Shopping List Creator
- **Summary**: My project allows the user to create a shopping list that will calculate how much their shopping spree will be. The values they input will be sent to the server, saved in appdata, and returned/updated to the client for a single-page app. Be sure to fill in the quantity and price tab with numbers (decimals are fine as well), otherwise you will not be able to properly find out the total price. 
- **CSS positioning techniques**: I used a CSS flexbox to center my project and make it look more refined. The .container class allowed me to move everything at once and it looked good already, so I did not create a .item class for individual sections. All fonts are linked from google fonts and Id, Element, and Class selectors are all used to reference different parts of the web page.


## Technical Achievements
- **Tech Achievement 1**: Using a combination of javascript and HTML, I was able to create a single page app. Whenever the user inputs data and presses the submit button, there is code in the javascript that will send the Client's POST to the server, which will update the appdata on the server. From there, there will be a promise that will call a GET that will get the appdata from the server and update the HTML on the screen (when submitting will only retrieve the new data), without needing to open a new page. In order to do this, I created an id inside the table in the HTML that would insert the data into a specific point of the table. Whenever the webpage is reloaded, a GET fetch is called that will retrieve any current data in appdata, and re-input the data into the table. When data is deleted, the client will send a POST to the server that will have the server filter through the current appdata and only keep any data that does not share the same shopping item name. Once the POST returns, there will be a promise that will call a GET fetch that will remove all the contents of the HTML table and re-input the appdata into the table.

### Design/Evaluation Achievements
- **Design Achievement 1**: 
