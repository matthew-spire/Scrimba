# The Frontend Developer Career Path

## Module 1 Welcome to the career path

### Welcome to the career path

#### 1. Welcome to the career path

- What you'll learn
  - HTML
  - CSS
  - JavaScript
  - React
  - Learn enough to get your first frontend developer job
- Might take a while, but "The best investment you can do"
- Founder's journey
  - Failed startup founder &rarr; Learned to code &rarr; Frontend developer (w/ lots of opportunities)
- Why learn this? Superpowers!
  - Freelance around the world
  - Financial independence
  - Make ideas come to life
- JavaScript is (ultimate) superpower
  - Billions (millions) of people use apps with and-or powered by JavaScript
  - People who know how to code JavaScript in the low millions &rarr; Superpower
  - Every industry must use the web &rarr; every industry needs JavaScript &rarr; in-demand

#### 2. About the path

- Fully self-paced
  - Watch the lectures and do the challenges
- Part-time or full-time
  - Minimum three months to complete (Do not rush!)
- Do something every day
  - At least during the weekdays &rarr; Will help with retention
- Scrimba is different
  - Video combined w/ code editor
    - Pause video at any given time &rarr; Jump into code editor and make changes &rarr; Changes reflected in real-time
  - Benefits of this approach
    - Coding > Watching &rarr; Learn code by writing code
    - Projects > Theory &rarr; Funner and see everything in context
      - First project is building a website that reflects your personality
        - Will not really know and-or understand what you are doing, but that is okay and expected
      - Next, get to the root of things w/ HTML and CSS by building a blog. Will also include design and best practices.
      - JavaScript and making websites interactive (e.g. forms)
        - Forms
        - Games (Pac-Man)
        - API-based apps (Random Programming Jokes)
        - Netflix clone
          - Database, User Auth, React
- Flow: HTML &harr; CSS &harr; JavaScript &harr; Project

#### 3. Meet your teachers

- Kevin Powell
  - CSS evangelist
  - 100k+ follow his YouTube CSS tutorials
  - In-person web development teacher
- Gary Simon
  - UI Design guru
  - 500k+ followers on YouTube
  - 100k+ (typo?) online courses and 20 years of experience
- Bob Ziroll (React)
  - Head of Education at V School
  - Turned 100+ students into frontend developers
  - Most popular React course on Scrimba and YouTube
- Cassidy Williams (React/Interview Prep)
  - ReactTraining.com
  - Netlify, Amazon, CodePen
  - Funny dev videos on Twitter
- Other instructors w/ small courses dealing w/ their specialty
  - Ebenezer Don &rarr; JavaScript
  - Jesse Hall &rarr; JavaScript
  - Dylan Israel &rarr; JavaScript
  - Ania Kubow &rarr; Games
  - Karl Hadwen &rarr; Netflix clone
- Per Borgen
  - Guide

#### 4. Discord + Email

- Scrimba Discord
  - Reach out, provide feedback, etc.
  - Chat application (think Slack, Teams, etc.)
  - Build a community to keep you company while you learn to code
    - Get involved &rarr; Stay motivated
    - Accountability
  - Introduce yourself &rarr;
    - introduce-yourself channel
    - today-i-will-learn channel &rarr; Commit to what you will learn that day (accountability)
  - share-your-code channel &rarr; Share your solutions to Scrimba challenges, see solutions from others, etc.
    - Sharing is good for feedback
  - Dedicated front-end path channel
    - Place for students to provide feedback, suggestions, etc.
    - Think of the course as a living organism
  - Help channels for different subjects
    - React, JavaScript, etc.
    - Community helps each other
    - Help others &rarr; Will help you learn
  - Pro Member tag
    - Join Discord
    - Add your username
- Email (every Monday)
  - Weekly encouragement
  - Bonus learning material (challenges)

#### 5. Join a study group

- Ability to join a study group
  - Private channel on Discord where you are grouped w/ other Frontend Dev. Career Path students
  - Connect, on a personal level, w/ others who are on the same path and probably struggling just like you are
  - Place that is safe enough to share struggles, successes, and projects
  - At least every Monday, someone from the Scrimba team will drop in and see how things are going, provide encouragement, etc.
  - Set aside time to code &rarr; Stick to the plan
- Should I join a Study Group?
  <ol>
    <li>Be active every week (leave a comment once a week)</li>
    <li>Add a profile picture</li>
  </ol>
- To join
  - Go to join-study-group channel on Discord
  - Post: I am interested in joining a study group! + Emoji of your choice
- More support

#### 6. Let's Make a Cake!

- Lot of stuff going on and may be overwhelming, but no need to understand majority right now
- Make a small modification
  - Hover over the egg and note the "scared" animation &rarr; look @ HTML code, see the egg, and also see "scared"
  - Change the egg's class from "scared" to "excited"
    - `<li class="scared"></li>` to `<li class="excited"></li>`
  - See notes by clicking on the hamburger menu in the bottom right
    - Can see the note by returning to screen cast where note was written as well as from the main menu (Where on main menu?)
  - Go into index.js and change the theme from 'light' to 'dark'
    - `setTheme('light')` to `setTheme('dark')`
- Click on settings wheel in bottom right corner to change font size, speed, etc.
  - Also where you can download the code as a ZIP

### Your first web app

#### 1. Add your Name and Emoji

- Web app that is personalized, unique, and just for you
- Technologies used to run the web app
  - CSS
    - Colors, backgrounds, fonts, variables
  - JavaScript
    - Conditionals, loops, fetch, functions
  - React
    - Props, APIs, hooks, JSX, state
  - Scary words &rarr; concepts and technologies that are being used to render the web app in the browser
    - Scary, but you need to get comfortable with the fact that when working as a frontend developer you are always standing on the shoulders of giants and there are always things going on under the hood that you do not understand
  - Have to accept that you will sometimes work on and-or with things you do not understand
    - ~80 lines of scary, hideous code you have to work w/
      - Limited to modifying a few lines
      - Only worry about/try to understand the lines you are modifying
- Make it your website
  - Change the name from 'Someone' to your name and change the emoji
    - `ReactDOM.render(<App name="Someone" emoji="👋" />, document.getElementByID("root"));` &rarr;
    - `ReactDOM.render(<App name="Matthew" emoji="🦄" />, document.getElementByID("root"));`
    - Can copy and paste an emoji from [getemoji.com](https://getemoji.com/)
  - Site is still boring, so we need to populate it with content

#### 2. Display Photos

- In index.js, the return(...); statement (function?) (i.e. the code) is set up to display pictures
  - No pictures are currently being displayed because there is nothing specifying what kind of photos to display on the website
    - Specify on line 24 of index.js
      - Uses a modern React concept called Hooks (Do not worry about this now, just be aware of it)
    - Set up the app so that it starts off with an initial state
      - Initial state &rarr; Whatever you put into useState("") on line 24 of index.js
      - Fill in w/ name of subject that you want your website to be populated w/ images of &rarr; refresh the code and observe the result
- How are pictures "magically" showing up on the page?
  - Use of an API (line 29 of index.js)
    - Unsplash is a website that contains free to use images
    - Our app sent a request to Unsplash requesting images &rarr; Unsplash said yes &rarr; Unsplash sent images of our specified subject back to our app &rarr; Our app took that date (images) and rendered out the photos
      - Using Internet infrastructure to construct something which pulls data from a third party source
- Now, change the background color, fonts, etc. to better match your subject selection

#### 3. Change the Background Image

- Personalize your website by styling it
  - Style websites by working with CSS (Cascading Style Sheets)
    - Go into style.css file
      - Note the background options under the root section (lines 3 through 12 of style.css)
      - Change the background to one you like
        - Modify line 44 of style.css
          - `--background-image: var(--wooden);` &rarr; `--background-image: var(--rainbow);`
      - Only changing what is in the var statements

#### 4. Choose a Color

- Change the font, border, etc. color to suit the subject you chose
  - Still in style.css
  - Note the color options under the root section
  - Modify line 49 of style.css
    - `--main-color: var(--snow)` &rarr; `--main-color: var(--gloom)`
- Important aspect of coding is that one variable can change many things on the page
  - Main reason we use variables

#### 5. Set the Font, Border, and Column Count

- Change the font family to one you like better
  - Still in style.css
  - Note the font options under the root section
  - Modify line 54 of style.css
    - `font-family: var(--simple-font);` &rarr; `font-family: var(--curly-font);`
- Adjust how many columns you would like to have
  - Modify line 60 of style.css
    - `column-count: 2;` &rarr; `column-count: 3;`
- Choose your favorite border
  - Uncomment the code (lines 71 and 73 in style.css)
  - Modify line 72 of style.css
    - Use the variables available for backgrounds
    - `/* border-image: var(--sweets) 100; */` &rarr; `border-image: var(--nightsky) 100;`
- Note how we modify different sections in style.css
  - E.g. body, grid, etc.

#### 6. Share your website

- Share your solution
  - Do the mini challenges (again) to make the website your style
  - Share a screenshot in the i-built-this channel on Discord
