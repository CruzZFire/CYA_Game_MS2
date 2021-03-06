# CYA_Game_MS2
Choose your adventure game (Milestone PJ 2 -CI FSC)

# Choose Your Adventure - The Long Lost Treasure
Pirate Game

**(MS interactive-front-end project - Code Institute by Ángel González)**

This is a "choose your own adventure" type of game. The game is both available to be played in browser of portable device. The site itself includes some optional access features like light/dark mode, sound effects and ambient music to personalise user experience.

---

## **Table of Contents**

1. [UX](#UX)
    * [User Stories](#User-Stories)
    * [Strategy](#Strategy)
    * [Wireframes](#Wireframes)
    * [Scope](#Scope)
    * [Structure](#Structure)
    * [Theming](#Theming)
2. [Features](#Features)
    * [Future Features](#Future-Features-Objectives)

3. [Testing](#Testing)
4. [Deployment](#Deployment)

    * [Github Pages](#Configuration-of-GitHub-Pages)
    * [Cloning Repository](#Cloning-the-Repository)

5. [Credits](#Credits)

    * [Images](#Images)
    * [Music](#Music)
    * [Acknowledgements](#Acknowledgements)

6. [Contact](#Contact)

---

## UX
### User Stories
Users of this WebApp will be people wanting to spend a good while playing through the game story and trying to beat it.

The site [(see full-size preview)](/assets/images/screencaptures/Full-page-browser.png) is based on a single interactive page. The sections are distributed symmetrically to make it intuitive to visually navigate through content in a fast and easy way.

Both the fonts and the optional ambient music are heavy pirate themed to make the experience more immersive for the user.

The user finds the game screen in the center of the window [(see full-size preview)](/assets/images/screencaptures/Full-page-browser.png) making it easier to focus on it.

Users also find the deployable card containing the "instructions" displayed by default, making it easy to understand how the game works in the browser.

Finally, the users have access to a deployable card containing some "options" to customize the experience both visually and audibly. [(see Features)](#Features)

### Strategy
The goal is that the user has a good time playing fluidly through the game. To achieve this, the design is clean and the theme is deeply defined. Also, some customize options are given to the user.

Another of the goals is that the player plays again after failing, so an option to "restart" is given right after losing. [(see Features)](#Features)

The most ambitious goal is having a player playing again after winning the game, to attempt to achieve this, four different endings were defined.

### Wireframes
Here are the first concept wireframes:

* [Browser-View](/assets/wireframes/Browser-idea.png "Browser View")

* [Device-View](/assets/wireframes/Phone-idea.png "Device View")

* Scene Types: 

![Scene-type-description](/assets/wireframes/Scene-type-description.png "Scene type description") 
![Scene-type-speech](/assets/wireframes/Scene-type-speech.png "Scene type speech") 
![Scene-type-combat](/assets/wireframes/Scene-type-combat.png "Scene type combat")

Final concept wireframes:

* Browser View: 

    ![Browser-View](/assets/wireframes/Browser-idea-defined.png "Browser View")

* [Device-View](/assets/wireframes/Phone-idea-defined.png "Device View")

* Scene Types: 

    See [Features](#Features)

Another very important part of the planning process was the structure of the story, this was in order to make easier establish code logic. Here are the decision trees of the game (last two are not included to avoid spoilers):

* Start decision tree: 

    ![Start-Tree](/assets/wireframes/Tree-decision-start.png "Start Tree")

* Hide decision tree: 

    ![Hide-Tree](/assets/wireframes/Tree-decision-hide.png "Hide Tree")

* Enlist decision tree: 

    ![Enlist-Tree](/assets/wireframes/Tree-decision-enlist.png "Enlist Tree")

* Rob decision tree: 

    ![Rob-Tree](/assets/wireframes/Tree-decision-rob.png "Rob Tree")

### Scope
Considering the goals set at [Strategy](#Strategy), it has been necessary to make a solid pirate theme [(see Theming)](#Theming) to make the experience coherent. As well as giving some options to customize and make the user spend more time in the WebApp.

Also, it was important to have all the interaction focused on the game screen to be able to use the project in portable devices.

### Structure
In the browser, all three main elements are occupying one third width of the screen:

  ![Full-page-browser](/assets/images/screencaptures/Full-page-browser.png "Browser View")

The **title** section, displays to the left and centered.

The **game** section, displays centered, focusing attention.

The **features** section, displays to the right with the instructions tab opened by default.

On a mobile device, all three main elements are aligned one on top of the other:

  ![Full-page-phone](/assets/images/screencaptures/Full-page-phone.png "Phone View")

The **title** section, displays on the top with reduced size.

The **game** section, displays centered and occupying most of the screen focusing attention.

The **features** section, displays under the main screen, given that this view is more intuitive and no space wants to be taken from the game section.

### Theming
As mentioned, theming was an important matter for the project in order to make the experience unique.

The special and more elaborated font for the title is [Jack Pirate](https://www.fontspace.com/jack-pirate-font-f42234) by [Måns Grebäck](https://www.fontspace.com/m%C3%A5ns-greb%C3%A4ck). The font for the rest of the site is "Pirata One".

All the pictures and designs were made in [Canva](https://www.canva.com/).

Color palette sticks to tones that are commonly associated with the pirate world.

Finally, the music used for ambience is [The Buccaneers Haul by Shane Ivers](https://www.silvermansound.com), meanwhile the sound effects were found at [Sound Snap](https://www.soundsnap.com/).

---

## Features
This site consists on a single page so let's focus on the different elements:

* **Site Icon**: a personalized WebApp icon displays on the browser. Also, it appears in the case someone bookmarks the game page.

    ![site-icon](/assets/images/site-icon.png "Site icon")

* Game **Title**: strongly styled as the [theming](#Theming) section explained. Display position adapts depending on screen size.

* **Game Screen**: display position adapts depending on screen size, keeping always the main focus spot. Here is the preview of how some of the different [types of scenes](#Wireframes) result, with changeable text on the interactive buttons and images on the background. As well as the text included in each different scene.

    ![Scene-type-description](/assets/images/screencaptures/Scene-type-description.png "Scene type description") ![Scene-type-speech](/assets/images/screencaptures/Scene-type-speech.png "Scene type speech")

    *Image*: background changes on every visited scene, making the story interesting and engaging, and the interaction meaningful.

    *Text*: changes along the image displayed are either a dialog or a description of the action. Both either prompting the player to take a decision or inform of the new circumstances.

    *Buttons*: the four buttons display the different options to take and they change according to the scene. The fact that sometimes not all of them are available, makes the user read and stop a second to engage deeper in the experience.

* **Miscelanea section**: placed to the right of the game screen, this card-panel system displays the game instructions by default to help the browser user understand the dynamic of the game. Once clicked, the "Options" card-panel displays and "Instructions" hides. On this panel the user finds sound and music management, as well as the option to change the theme to a darker one. The active option is marked by an underline.

    ![Features-default](/assets/images/screencaptures/Features-default.png "Features default") ![Features-options](/assets/images/screencaptures/Features-options.png "Features options")

    *Sound Effect*: "ON" by default, allows to mute the sound effect when changing scene.

    *Ambient Music*: "OFF" by default, allows to play pirate themed music as background while the user is on the site.

    *Light Mode*: "ON" by default, allows to change the site background to a darker version to reduce the light coming from the screen.

* **Hover Effects**: there is a slight shading in the game screen buttons on browser when the user scrolls over them while deciding. There is also a hover effect over the "Miscelanea section" titles and "Options" text changing colour. This effect along with the mouse transforming to pointer makes it clearer to the user that some action is available, apart from the aesthetic, of course. 

* **Inside the Game**: a bit of explanation of what it is in the actual game.

    *Base Dynamic*: the premise of the game is choosing an option in a situation and progress to another.

    *Deaths*: there are nine different deaths to close different story arcs. After each of them, the user gets prompted to "Restart" by including it as the only option in the interactive buttons.

    *Wins*: after finishing successfully the correct arc, the user gets to choose fours different endings. After the chosen ending is viewed, the player gets prompted to play again to see another ending by including "Play Again" as the only option in the interactive buttons.

    *Battle mode*: special mode with slightly different mechanics. Player is trapped in this scene until victory or defeat. Turn based battle to the best to five, which is the number of lives provided for both player and opponent.

The whole site has response from small devices to larger screens, moving sections from sideways to top/bottom when needed to achieve the best display. It is not responsive on 4k at the moment.

### Future Features Objectives
Ordering the possibilities in a list of viability, considering both complexity and relevance:

1. Creating parallel partial story arcs, adding complexity to the global story arc of the game. (LOW complexity / MED relevance)

2. Adding a trophy system to the bottom of the page, unlocking them when a player reaches a certain death, a certain number of deaths, a certain win, etc... (MED complexity / MED relevance)

3. Save game feature allowing the player to save the current situation on the story and coming back another day or in another terminal. This is provided the points 1 and 2 are implemented. A login system. (HIG complexity / MED relevance)

4. Provide proper sizing and response for 4k screens (MED complexity / LOW relevance)

---

## Testing
During the development phase, using Brackets by Adobe and its built-in live preview made it very easy to adjust response and test the majority as was coded, via Developer Tools.

After finishing the coding, used "HTML validators", "CSS lint" and "JS hint" checking for possible warnings or errors.

>Note: as no modules (import/export) are being used for this project but diverse .js files are implied, a file called *.jshintrc* was created to reduce some errors called by the JShint built in on Brackets.io. Even with this fix, some redeclaration warnings are still shown.

**Global Display:** tests were made on browsers (Chrome, Edge, Firefox), tablets and phones ensuring responsiveness of the WebApp on every screen size. Some examples of portable devices used by testers involved or myself were:

 * Huawei Mate 9 Lite, Huawei GR5 2017
 * Apple iPhone 11
 * Apple iPhone 8
 * Samsung Galaxy A50
 * BQ Aquaris M10 Ubuntu Edition
 * Microsoft Surface 2
 
**Game Screen:** display of every single scene of the different story arcs needed to be tested. For this purpose I counted with the help of some Beta-testers.
>Note: history of the errors can be seen on [*Phase 1*](/assets/tests/Phase1.png), [*Phase 2*](/assets/tests/Phase2.png), [*Phase 3*](/assets/tests/Phase3.png).

**Game Commands:** the same way as the screen, load of the proper button text and interaction had to be tested, so once more I counted with the help of some Beta-testers.
>Note: history of the errors can be seen downloading the spreadsheet in the "./assets/tests" path of the master branch.

**Options:** music and sound effects were tested on different devices as well. The same with the different available backgrounds.

**Links:** a single external link is present. It was tested after deployment at GitHub Pages.

---

## Deployment
This site is temporarily hosted on GitHub Pages, from Master branch. 

Deployment on Pages was made only before submitting the project for final testing. The project was kept on Brackets "live preview" for modifications, even though it was committed to GitHub and updated via GitBash on a frequent basis.

#### Configuration of GitHub Pages
1. Enter the repository *Settings*.
2. Scroll down to the *GitHub Pages* section.
3. Locate *Source* dropdown menu and select *'Master Branch'*.
4. After scarce time, the link is available and working. [*Access here*](https://cruzzfire.github.io/CYA_Game_MS2/).

#### Cloning the Repository

To run it on your local computer offline, the repository must be cloned beforehand.

1. Once on the repository locate the *Clone or Download* dropdown menu.
2. Copy either the HTTPS or SSH route to your clipboard.
3. Open *GitBash* and move to the folder where you want to place the cloned repository files.
4. Type **"git clone"**, **tap spacebar once** and then paste the route copied in your clipboar at *step 2*.
5. Press Enter to exec the command and the local cloned files will be created.

---

## Credits

All the ideas, materials displayed and all the site designs belong to Ángel González. Only exception is the "ambient music" [see Theming](#theming).

### Images
[*Canva.com*](https://www.canva.com/)

### Music
[*The Buccaneers Haul by Shane Ivers*](https://www.silvermansound.com)

**Disclaimer:** This site and its contents or any portion thereof may not be reproduced or used in any manner whatsoever without the express written permission of the publisher except for the use of brief quotations as credits and/or recommendation. Copyright © 2020.

### Acknowledgements
Great help once more from the documentation of these two sites, you can really learn as you go and adapt their examples to your own code:

    * [w3schools](https://www.w3schools.com/)
    * [MDN](https://developer.mozilla.org/en-US/)

Special mention to this page for providing pirate themed slang:

* [Pirate Voyages](https://www.piratevoyages.com/pirate-lingo/)

Also a shoutout to my mentor on this project [Maranatha A. Ilesanmi](https://github.com/mbilesanmi) for providing guidance when needed.

---

## Contact

**E-mail:** a.cruzana88@gmail.com :technologist:
