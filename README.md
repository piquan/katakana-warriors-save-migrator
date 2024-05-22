# Katakana Warriors Save Migrator

Welcome to the Katakana War Save Migrator, a tool designed to
facilitate transferring save files between the standalone
application and an alternative web-based version of the
[“Learn Japanese To Survive! Katakana War”](https://store.steampowered.com/app/554600/Learn_Japanese_To_Survive_Katakana_War/)
game. This utility helps navigate around technical issues encountered
in the standalone version by making use of the game’s inherent web
compatibility.

**Important Disclaimer:** This utility operates independently and is
not endorsed by Sleepy Duck or River Crow Studio, the game’s
developers. For official game-related merchandise or to support the
creators, please visit https://study-japanese.net/

**Background on Game Versions:** “Learn Japanese To Survive!  Katakana
War” is primarily a standalone game. Although it operates mainly as a
desktop application, its architecture is based on web technologies,
housing a “www” subdirectory that can function directly in web
browsers. This setup isn’t a separate web version per se but rather
the same application accessed through a browser via a local
server. This method is not officially documented or supported but is
entirely feasible. It does, however, manage its save games differently
than the standalone mode.

**Why This Utility Exists:** Sometimes the standalone version of the
game works great, but other times you might run into weird glitches or
issues, especially if your system setup is a bit unusual. If you find
the game runs smoother in your web browser, or if you just prefer
playing there, this tool makes it easier to move your save files back
and forth. It’s handy for keeping your game going, no matter where you
choose to play.

## How to Use

1. **Back Up Your Game Data:** Before proceeding, ensure you back up
your game data to avoid any accidental loss.
[Here’s how to back up your game.](https://help.steampowered.com/en/faqs/view/4593-5CB7-DC3C-64F0)
This Save Migrator utility has not been extensively tested and could
potentially affect your saves or the app itself.

3. **Prepare the Utility:** Download
[`save-migrator.html`](save-migrator.html?raw=true)
and place the file in the app’s `www` directory. For example, the path
might be
`~/.steam/steamapps/common/Learn Japanese To Survive! Katakana War/www/save-migrator.html`

5. **Set Up the Server:**

   1. Open a terminal window.

   2. Change the directory to where you’ve placed the file, using
   `cd ~/.steam/steamapps/common/Learn Japanese To Survive! Katakana War/www`
   
   3. Start a local server by running: `python3 -m http.server -b localhost`
   
6. **Access the Utility:** Open your web browser and go to
http://localhost:8000/save-migrator.html to access the utility.  The
game normally uses Chromium internally, so you may want to use Chrome.

The rest of the directions are in that page.

## License

Copyright © 2024 Joel Ray Holveck

This program is solely the creation of Joel Ray Holveck. It is not
affiliated with, endorsed by, or approved by Sleepy Duck and River
Crow Studio, nor is it connected in any way with the employers of
Holveck.

This program is licensed under the [MIT License](LICENSE).
