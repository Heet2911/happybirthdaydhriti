DHITTU'S BIRTHDAY SURPRISE — QUICK EDITING GUIDE

FILES
- index.html: the entire website. HTML, CSS and JavaScript are all here.
- assets/: put Dhittu's photos and one MP3 song here.

THE EASIEST WAY TO PERSONALISE
1. Open index.html in VS Code (or any text editor).
2. Search for: EASY EDIT ZONE.
3. Edit only the CONFIG object in that section. You do not need to touch the rest of the code.
4. Save, then double-click index.html to preview it in your browser.

PHOTOS — ADD AS MANY AS YOU LIKE
- Cover photo filename: dhittu-cover.jpg
- Gallery photos: photo-01.jpg through photo-09.jpg are already listed as examples.
- Put your real pictures in the assets folder and use those exact filenames, or change the filenames in CONFIG.
- To add a 10th photo, add this inside the memories array (before its closing ]):
  { photo:"assets/photo-10.jpg", caption:"your caption here" },
- Repeat for photo-11.jpg, photo-12.jpg, etc. There is no fixed photo limit.
- JPG, PNG and WebP work if the filename/extension in CONFIG matches your file.

WRITE A LONGER LETTER
- Add more quoted paragraphs inside letter: [ ... ].
- Each paragraph is a separate string, separated by a comma.
- Example: "One more thing I love about you is...",

ADD TIMELINE MOMENTS
- Add another object inside timeline: [ ... ]
- Example: { date:"14 February", title:"Our favourite day", text:"Write your memory here." },

EDIT THE MINI QUIZ
- Each quiz item has a question, three or more options, answer and correct message.
- answer is the option position starting from 0: first option = 0, second = 1, third = 2.

OTHER SETTINGS
- herName: displayed name (currently Dhittu).
- passcode: exactly four digits. Currently set to 0000 as a placeholder — change it!
- songTitle/songArtist: text shown above the player.
- songFile: put an MP3 at assets/our-song.mp3, or change the path.
- giftMessage, finalMessage, finalSignature: edit the surprise text.

HOW THE CODE WORKS
- HTML defines the different screens and buttons.
- CSS creates the soft pink scrapbook design, responsive layout and animations.
- JavaScript reads CONFIG and builds the letter, photo gallery, timeline and quiz.
- The keypad compares the four digits with CONFIG.passcode.
- The gift opens on tap; the final button creates a confetti/heart celebration.

IMPORTANT NOTES
- The passcode is a playful entrance only, NOT real security. It is visible in the source code.
- The website works locally. To share a public link, publish the folder to GitHub Pages or Netlify; keep index.html at the root and upload the assets folder too.
- Browsers may block autoplay. She can press play herself.
- Use photos and music you have permission to share. Avoid posting private photos publicly without her consent.
