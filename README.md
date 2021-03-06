# MMrY - The Christmas Memory Game.

### Welcome to MMrY. 
**MMrY**, a very original short name for Memory. It is a small and easely understood game that is developed with the goal to create an accesible environment to keep your brain on top. 
This game is part of a project done during a Full Stack Dev Course supplied by Code Institute©. Both me in the role as creator and the Institute has full rights to this projects, to clone or fork the repository on [GitHub](https://github.com/Daffie95/MS2-mmry).
Below will be a full summary of the project, from a creation stage and following trough to a finished project. 
<br>
<br>
As a small disclaimer this is a continuation of a previously failed project and old files can be found in the _Old directory.

### Table of Contents.
#### 1. Project Planning.
#### 2. Updates Timeline.
#### 3. Planned Updates.
#### 4. Bugs & Errors.
#### 5. Additional Comments.
#### 6. Testing.
#### 7. Conclusion.

# 1. Project Planning.
The idea for this project came to me when I had a discussion with a friend about dementia, and how small and continous activation of the brain does tremendous work to battle dementia.
So I decided that my Project would be a memory game. Memory games are usually small and consize of a number of cards that all has a matching counterpart. So to finish the game the user will need to find every two paris of card in the game to complete it.
All the cards will have the same backside to not visualy disrupt the game or make it unclear, while as mentioned above there will be 6 different cards, each with another exact match, giving us 12 cards in the game. 
<br>
<br>
Inital wireframes of the project can be found in  /Wireframe. Thanks goes out to UXPin for allowing me to use their software.
<br>
<br>
There are different techniques to make this project work. The webpages, the landing page and the game page will consist of HTML and CSS to create an intuitive layout and easy on the eyes design. 
I dont want to complicate things, as the target audience might be individuals that struggles with disorders, and may not handle aggressive color palettes very well. 
Alongside the  HTML and CSS the main functionalities will be utilizing JavaScript to create a functional memory game.
<br>
<br>
Using a JavaScript function that counts the card and the given ID (I will use the Data attribute to connect the HTML element with the JavaScript Funtion), the function will initially shuffle each card on load and only shuffle if the page is refreshed and/or the 'Restart' button is pressed.
There will be roughly about 5 different functions needed to create a finished project. One to  allow cards to flip, one to check for a match between the two flipped cards, one to disable the two clicked cards if the cards match, and one to unflip cards if they dont match, and finally a function to shuffle all the cards upon loading the page.


# 2. Updates Timeline.
> ### *1.0 Deploy Version*
> Removed comments from gamepage.html <br>
> Removed comments from index.html <br>
> Removed comments from scripts.js <br>
> Removed comments from styles.css <br>
> Moved styles.css and scripts.js into /assets
> Corrected links to /assets for scripts.js and styles.css
> file links now work as intended.

> ### *0.9*
> Removed placeholder text in index.html and updated with current information.<br>
> Added clickable lists of resources to landingpage.<br>
> Uploading .TXT files that I saved code in before GitPod stopped working to /txt-saves. (Read Additional Comments)
> Updated Meta desc, Meta tags, Meta Author across page.

> ### *0.8*
> Reworked Buttons to make the entier button a clickable link<br>
> Changed coloring on buttons.<br>
> Added a JS Refresh to the restart button.<br>
> READ 6. Additional Comments for 2021-02-08<br>

> Fixed layout for Updates Timeline.<br>
> Added current README.md in from before GitPod went down. (Read Additonal Comments)<br>
> Added current scripts.js in from before GitPod went down. (Read Additonal Comments)<br>
> Added current index.html in from before GitPod went down. (Read Additonal Comments)<br>
> Added current gamepage.html in from before GitPod went down. (Read Additional Comments)<br>
> added current styles.css in from before GitPod went down. (Read Additional Comments)<br>

> ### *0.7*
> Updated layour and color palette. <br>
> Added a landingpage. <br>
> Added styling to Landing page. <br>
> Added Navigation between landingpage and gamepage. <br>
> Styled the Landingpage. <br>
> Added comments to new elements. <br>
> Fixed Scaling issues where cards would span outside of the screen on smaller devices. <br>
> Fixed Image rendering on smaller devices <br>
> Updated and Organized 2. Updates Timeline.
<br>

> ### *0.6*
> Moved previous README.md to _Old/ and added it to .gitignore <br>
> Created a new README.md to match current project.  <br>
> Updated the new README.md with Table of Contents. <br>
> Updated the new README.md with a more detailed Planning section. <br>
> Uploaded a wireframe to the Wireframe/. <br>
> Added Updates from _old-README.md to README.md. <br>
<br>

> ### *0.5*
> updated colors<br>
> included a shuffling function using flex-items internal hierarchy<br>
> tried re-refactoring to see if primaryCard bug persists<br>
> updated code to stop matched cards from being clicked again<br>
<br>

> ### *0.4*
> retried refactoring of JS functions and now works.<br>
> Reverted back to before refactured due to bugs or breaking the code<br>
<br>

> ### *0.3*
> ending work<br>
> refactured functions in *scripts.js*<br>
> removed scripts2.js<br>
> fixed errors * 1. & 2.*<br>
> added resources used<br>
> moved projects to VSCode<br>
<br>

> ### *0.2* (23-12-2020)
> set a timeout for when cards are not matching, so we are still able to see what card we click (fixed)<br>
> Testing matching the cards using the data-* HTML attribute<br>
> Updated element classes to easely be difined in *index.html* & *styles.css*<br>
<br>

> ### *0.2* (22-12-2020)
> updated depth and 3d effects in *styles.css* for selector and .memory-cards<br>
> tested the targeting selector for the function to flip the cards<br>
> added querySelectorAll to target .memory-cards in *index.html*<br>
> starting script formating in *scripts.js*<br>
<br>

>  ### *0.1* (22-12-2020)
> updated *styles.css* with comments<br>
> added active transition<br>
> added hover transition<br>
> updated cards position<br>
> updated position of section element<br>
> added color to card background<br>
> added colors to background <br>
> added images for front and back cards <br>
> updated *index.html*<br>
> added *index.html*, *styles.css*, *scripts.js*.

# 3. Planned Updates. (In order of prioritization)
1. ~~Add a landingpage to match wirefram.~~
2. ~~Add a functional restart button to game page.~~
3. ~~Fix error where players can break out of the fuction that clicks the cards.(read more in 4.)~~
4. ~~Add notification upon completing the game. (if time allows)~~ It did not.
5. ~~Update anchor link tags on the restart button on gamepage.html~~


# 4. Bugs & Errors.
> 1.
>> **Expected Result:**
Clicking a card 3 times without finding the correct match should continue to turn the card face down.
>> **Actual Result:**
Clicking the card 3 times locks the card you clicked the first time. 
>>> Conclusion: This error is resolved, but was fixed back when I used VSCode and I had troubles connecting to Git to push commits.

>>> Fixed: yes (2021-02-05)

> 2.
>> **Expected Result:**
The card you click regardless of which of the 12 cards you click will call the EventListener.
>> **Actual Result:**
The first clicked card always fires as if the EventListener is stuck firing on the card the user clicked first.
>>> Conclusion: - This error has been resolved. Similarly to *1.* this was fixed used VSCode and I had issues connecting it to Git.

>>> Fixed: Yes (2021-02-08)

> 3.
>> **Expected Result:**
Clicking 2 cards will not allow user to click more cards to break the function of the game.
>> **Actual Result:**
Clicking 3 or more cards will continue to unflip cards and break the loop. 
>>> Conclusion: While cleaning up the code the error fixed itself, leaning me towards the conclusion that it was an indentation error along the road.

>>> Fixed: yes (2021-02-08)

# 5. Additional Comments.
> ## 1.
> *2021-02-08 / 22:05*<br>
**GitPod is having issues with connectivity, preview is buggy and commits are not going trough. I will add "commits" below here for clarity.**<br>
> Changed the buttons to not change color on hover<br>
> Added a zoom when hoving on buttons.<br>
> added padding to button anchor text to span the entire button, making the entire button clickable.<br>
> Updated **0.8*<br>
> Added 7. Testing section to README.md.<br>
> Revisited lockBoard variable in scripts.js and resolved an error allowing users to break out of the functions that locks unclicked cards when during the matching function.<br>
> Added above mentioned error in the 4. Bugs & Error because I forgot.<br>
> Cleaned up scripts.js (formatting).<br>
> Because I am currently unable to push to GitHub I have also saved all code in notepads to not lose everything (not kidding) (2021-02-08 23:14)<br>
> Gitpod is now working again after a hard reset and restart. There will be gaps in the commits between ~22:05 when I realised and 23:14.<br>
> Working on pasting my saved code back into GitPod.<br>

> ## 2.
> *2021-02-09 / 12:09* <br>
> There are unresponsiveness issues only visible on phone devices. The error is that the primaryCard thats clicked (i.e the first card)
becomes unclickable once the cards turns face down again. secondaryCard works as intended.
However, I dont have any experience in troubleshooting on mobile devices as the DevTools is not giving me any errors. The final console.log()
is fired indicating that the board is unlocked, but it seems like the lockedBoard function is still applied to primaryCard once the classList.Toggle"flip" is untoggled by the timer in flipUnmatchedCards.
this renders the user unable to click the primaryCard two tries in a row. 
<br>
<br>
I am very unsure how to deal with issues like this. As I dont think its something the course has gone trough. 
While testing from GitHub pages, I get one results. While testing from my private phone I get another result (which is not better by the way).
How am I supposed to troubleshoot different errors doing different things on different devices? There isnt really any time for me to fix this as the deadline is coming up in 39 minutes. 
I will be removing the paragraph on index.html advicing users to use their phone on the page. 


# 6. Testing.
> ## 1.
> **GitPod Issue. 2021-02-08 ~23:30**
>> Roughly at 22:00 GitPod became unresponsive. Preview port became disconnected and Terminal would not connect to my workspace.<br>
So I decided to back-up my work in TXT files (can be found in /txt-backups) to save me from losing all my changes made.<br>
This is simply testing every that it works as it should and did before the hard restart of Gitpod. This is not Final testing.
>>> *index.html looks like before hard restart:*
>>>> Yes but Navigation has reverted back to showing overflow of the elements making the screen fluttery when hover. Most likely an error in styles.css.<br>
**Fixed by re-applying box-sizing to body**<br>

>>> *gamepage.html looks like before hard restart:*
>>>> **Yes and with fixing index.html box-sizing in styles.css it was fixed on gamepage.html aswell.**

>>> *styles.css looks like before hard restart:*
>>>> **Yes and with fixing the box-sizing for index.html and gamepage.html all 3 works accordingly.**

>>> *scripts.js works like before hard restart:*
>>>> **Yes, scripts for the game works as intended**

# Final Testing.

> ### Grammar and readability check for text content: 
> ![Grammer Check Using Grammarly](https://i.gyazo.com/86d87b280f556675177a452ec155a460.png "Grammar Score")
> ![Readability Check using WebFx](https://i.gyazo.com/69eb865e8ba24fc5a9eb45b3c4e09dc6.png "Readability Score")

> ### User Experience Testing:
>> Are all anchor links functional, and/or opens in a new tab when opening a new webpage?<br>
**YES** <br>
>> Are all 12 cards on gamepage clickable?<br>
**YES** <br>
>> Can users only flip 2 cards at a time?<br>
**YES** <br>
>> Does flipping 2 match the cards and removes the function to click them again? <br>
**YES** <br>
>> Does the flipping function work troughout untill all cards are matched and flipped face up?<br>
**YES** <br>
>> Does the restart button refresh the page?<br>
**YES** <br>
>> Does the restart buttong run the javascript function to shuffle the cards? <br>
**YES** <br>
>> Is the core memory game functional on smaller screen devices. <br>
**The game is fully functional, however the scaling of the container and its child elements makes the layout squished** <br>

> ### Performance Testing:
>> ![Performance Test Using DevTools Performance](https://i.gyazo.com/d23edfe19068b9d7805cc8b701b39f9a.png "Tested by clicking links and flipping cards")<br>
>> [Performance Test For index.html using webpagetest.org](https://www.webpagetest.org/result/210209_DiGF_308357213ec2543adda7a58826bf349f/)<br>
>> [Performance Test For gamepage.html using webpagetest.org](https://www.webpagetest.org/result/210209_DiBN_be4041f0b5518e7ed1f56d516a8a01af/)<br>
> ### HTML Validator:
>> [HTML Validator for index.html](https://validator.w3.org/nu/?doc=https%3A%2F%2Fdaffie95.github.io%2FMS2-mmry%2Findex.html)<br>
>> [HTML Validator for gamepage.html](https://validator.w3.org/nu/?doc=https%3A%2F%2Fdaffie95.github.io%2FMS2-mmry%2Fgamepage.html)<br>
> ### CSS Validator:
>> [CSS Validation for index.html](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fdaffie95.github.io%2FMS2-mmry%2Findex.html&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=sv)<br>
>> [CSS Validation for gamepage.html](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fdaffie95.github.io%2FMS2-mmry%2Fgamepage.html&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=sv)<br>

> ### JaveScript Validator:
>> unable to find an easy to use JS tester to test the functionality of the scripts.js in conjuntion of the html pages.
> ### Google Lighthouse Diagnosis:
>> [Google Lighthouse Report for index.html](https://i.gyazo.com/bec1f4918d530fcea22eb70017f485e7.png)<br>
>> [Google Lighthouse Report for gamepage.html](https://i.gyazo.com/55c715d2553c42c30a7301689076cb65.png)

# 7. Conclusions.

I know that these times are really strange with a huge pandemic going on forcing isolation on people. Its been very hard for me to balance studying and the new real life things I have to deal with currently.
However, I feel very satisfied with solving the issues that came from submitting a poorly designed and executed Milestone Project. There were small errors breaking the flow of the Memory Game, later deducted to stem from indentation issues, that's now solved and the game works as intended.
I am happy I took a "very bad" project and tourned it around (*atleast in my eyes*) to hopefully recieve a passing grade.
<br>
<br>
I would like to give thanks to the Student Counceling from Code Institute that help me plan out my continuation of this project. Aswell as UXPin for giving me a student pass for using their premium software and services.