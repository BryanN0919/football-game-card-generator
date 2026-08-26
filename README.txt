FOOTBALL GAME CARD GENERATOR — VERSION 9

This version recreates the updated dashboard design and printable card layout.

FEATURES
- 4-person crew
  Referee
  Umpire
  Head Linesman
  Line Judge

- 5-person crew
  Referee
  Umpire
  Head Linesman
  Line Judge
  Back Judge

- 7-person crew
  Referee
  Umpire
  Head Linesman
  Line Judge
  Back Judge
  Field Judge
  Side Judge

CARD DESIGN
- 4 cards on one US Letter 8.5 x 11 page
- Thick black horizontal line above the gray game-information section
- Thick black horizontal line below the gray game-information section
- Gray background for teams, date, kickoff, and location
- Official names use Arial 20 pt-equivalent CSS sizing for 4/5-person cards
- Position labels use Arial 18 pt-equivalent CSS sizing for 4/5-person cards
- 7-person cards automatically reduce those sizes slightly so all seven positions fit
- Reduced unused white space in the officials section

WEBSITE FEATURES
- Updated navy dashboard design
- Crew-size toggle buttons
- Live card preview
- Home and away teams
- Date, optional kickoff time, optional location
- Change/reset association logos
- Automatically remembers game settings and official names in local browser storage
- Print button
- Direct Download PDF button
- Clear All button

RUNNING THE SITE
1. Unzip this package.
2. Keep index.html, cfoa.png, and chsaa.png in the same folder.
3. Open index.html in Chrome or Microsoft Edge.
4. Enter the game and crew information.
5. Use Print or Download PDF.

DIRECT PDF NOTE
The Download PDF button uses html2canvas and jsPDF from cdnjs.com.
Internet access is needed for those two libraries when opening the site locally.
If the libraries are unavailable, use Print -> Save as PDF instead.

RECOMMENDED PRINT SETTINGS
- Paper: Letter
- Orientation: Portrait
- Margins: None
- Scale: 100% / Default
- Headers and footers: Off

HOSTING
The site is static and can be hosted on:
- GitHub Pages
- Azure Static Web Apps
- Netlify
- Any ordinary web server

No backend or database is required.


VERSION 5 UPDATES
- 7-person crews no longer scale the official names or position labels down.
- All crew sizes use Arial 20px for official names.
- All crew sizes use Arial 18px for position labels.
- The gray game-information band has been moved farther down by increasing the logo area.
- Added more vertical spacing beneath each official row for improved readability.
- Increased the thick black divider lines above and below the gray section.
- 7-person cards use tighter internal spacing only; typography remains unchanged.


VERSION 6 UPDATE
- The 7-person card now uses exactly the same card layout as the 4-person and 5-person cards.
- No special 7-person logo height, game-information spacing, crew padding, or row spacing is applied.
- All crew sizes use the same:
  * Logo/header dimensions
  * Gray game-information band position and dimensions
  * Thick black divider lines
  * Crew section padding
  * Vertical row spacing
  * Arial 18px position labels
  * Arial 20px official names
- The only difference between crew sizes is the number of official rows displayed.


VERSION 7 UPDATE
- Added a clock icon immediately before Kickoff Time in the gray information section.
- Added a home icon immediately before Game Location in the gray information section.
- Icons are inline SVG graphics, so they print sharply and are included in downloaded PDFs.
- The icon rows only appear when the optional kickoff time or game location is entered.


VERSION 8 PRINT FIX
- Added CSS print-color-adjust rules so the gray game-information band is preserved when printing.
- Added explicit print-time gray background styling for Chrome and Edge.
- The direct Download PDF button already captures the gray background.

IMPORTANT BROWSER PRINT SETTING
Some browsers can still suppress background colors unless "Background graphics" is enabled.

Chrome / Edge:
1. Click Print.
2. Open More settings.
3. Turn ON "Background graphics".
4. Print or choose Save as PDF.

For the most consistent output, use the green Download PDF button, which renders the card backgrounds directly into the PDF.


VERSION 9 DIRECT-PDF FIX
- Fixed a common direct-PDF failure when the generator is opened locally by double-clicking index.html.
- Default CFOA and CHSAA logos are now embedded directly into the page for PDF rendering.
- This prevents the local file:// image security/CORS issue that can cause html2canvas to fail.
- The PDF generator now waits for all logos to finish decoding before capturing the page.
- Uploaded custom logos continue to work because they are converted to browser-safe data URLs.
- Print/PDF gray-background fixes from Version 8 remain in place.

NOTE
The jsPDF and html2canvas JavaScript libraries are still loaded from cdnjs.com, so internet access is required for the green Download PDF button. Normal browser Print does not depend on those libraries.
