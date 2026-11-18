FIVE CAR RALLY — GitHub Pages edition

LATEST UPDATE
- A finishing card can still swap before points are awarded.
- Example player names: Anabella, Amy, Riley.
- Claim limits: 2–3 players = 1 spot per color; 4–7 = 2; 8–15 = 3.
  Solo practice remains available with 1 spot per color.
- The five cars are red, blue, green, orange, and purple.
  Old black cards/cars are orange; old gray cards/cars are purple.
- Each space shows number and arrow first, points second, special label third.
- Numbers/arrows/labels remain 22px; points remain 28px.
- Cars slide through every intervening space, including backward movement
  and row turns. Other controls wait until the slide completes.
- Round 3 shows the doubled point values directly on the track.
- Existing saved games retain their scores and positions with updated colors.

OFFLINE PLAY ON IPAD
1. Upload all files in this ZIP to the same GitHub Pages folder.
2. While connected to Wi-Fi, open the published game link in Safari.
3. Wait for the message: Ready for offline play.
4. Tap Share > Add to Home Screen (look under More if needed).
5. Enable Open as Web App if shown, then tap Add.
6. Open the new Car Rally icon once while still connected to Wi-Fi.
7. Wait for Ready for offline play inside that app too.
8. Turn on Airplane Mode and verify the game reopens from its Home Screen icon.

The ZIP alone does not install the game on an iPad. The first setup uses the
published HTTPS game link. After setup, all three rounds can run offline.
Clearing website data removes the offline copy and stored progress. Keep
this ZIP so you can set it up again. Opening from the Home Screen may use
separate saved progress from an existing Safari session; finish any ongoing
game first and use the Home Screen icon consistently afterward.

To update the installed copy later, connect to Wi-Fi, open the game, then
close and reopen it after the updated offline files have finished installing.
Whenever changing the game code in the future, also change the cache version
in sw.js so the installed app caches the new index.html.

Apple Home Screen instructions:
https://support.apple.com/guide/ipad/ipad8f1f7a29/ipados

GET STARTED
1. Extract this ZIP on your computer.
2. Open your GitHub repository (or create a new repository).
3. Upload ALL seven game files to the top level of the repository and commit:
   index.html, sw.js, manifest.webmanifest, icon-192.png, icon-512.png,
   apple-touch-icon.png, and README.txt. Keep their exact filenames.
4. In the repository, open Settings > Pages.
5. Under Build and deployment, select Deploy from a branch.
6. Select main (or the branch containing index.html), choose / (root), then Save.
7. When GitHub shows the published address, open that address in Safari on your iPad.

All game and offline files are included. There are no external services,
spreadsheets, accounts, or server code required by the game.
The 70 supplied cards and all 18 supplied spaces are built in.
GitHub instructions reference:
https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

PLAY
Enter 1–15 player names, one per line. Players take turns in that order.
Tap Draw card and follow the controls. Roll your real die only for a roll card,
then tap -1, 2, 3, 4, 6, or star. Wild cards let you select any car.
Use End turn when done. Use Undo to correct mistakes in the current session.
At round end, review points and tap Start round 2 or Start round 3.

FIVE SHARED CARS
There are always exactly five pieces: red, blue, green, orange, and purple.
A random assignment is made each round from a pool with:
  2–3 players: one assignment slot per color
  4–7 players: two assignment slots per color
  8–15 players: three assignment slots per color
Unfilled slots remain available for swaps. Multiple players can share the exact same car.
A car moves once when a card moves it. All its players receive its final points.
Cards can move cars that belong to other players, or unclaimed cars.

SWAPS
A swap is optional and happens after the card's movement.
The current player may switch their OWN assignment to another color with an
open claim spot. Each color has 1 spot for 2–3 players, 2 spots for 4–7
players, or 3 spots for 8–15 players. A color can be available even when
another player already shares that car. Full colors cannot be chosen.
A swap frees the player's old spot and claims one spot on the new color.
Other players keep their assignments. No car changes position due to a swap.
With 15 players, all 15 spots are filled, so no swap is available.
Swap buttons show the number of open spots; car labels show claimed/total.

MOVEMENT AND ROUND END
Stars are spaces 5, 9, 13, and 15 (START is space 1).
A star card or star die result goes to the next star strictly ahead.
If there is no star ahead, the car stays put. A swap can still be taken.
Hotdog stand is space 7. Hotdog cards move there from either direction.
Go-to-color cards move to that color's exact space, forward or backward.
Negative moves stop at START; they never go behind it.
All five cars start each round at START. All 70 cards are shuffled each round.
If the deck runs out, discards are shuffled and the same round continues.
Reaching or passing space 18 (FINISH) ends the round immediately, even if
that car has no players. If the finishing card has a swap, the current player
may still swap to any color with an open spot before points are awarded.
Keeping their car skips that swap and scores the round. No extra turn follows.
Points use the assignments AFTER that final swap. This also applies in round 3.

POINTS
Spaces 1–6: 1 point
Spaces 7–10: 2 points
Spaces 11–13: 3 points
Spaces 14–15: 4 points
Spaces 16–17: 5 points
Space 18: 7 points
Rounds 1 and 2 award those values; round 3 doubles them.
Each player earns the value of their assigned car's ending space.
The three rounds are added together. Tied leaders share the win.

DEVICE NOTES
Use one shared iPad. Separate devices do not synchronize.
Progress automatically saves in this browser on this device when browser
storage is available. Clearing website data clears saved progress.
Undo history lasts until the page is refreshed or closed.
To start fresh, tap New game. Use the Car Rally Home Screen icon for offline play.
This version is designed for iPad touch use; physical iPad/Safari testing
was not available during creation.

RULE INTERPRETATIONS
These choices were necessary where the supplied rules did not specify:
- START is the first listed 1-point space (18 total spaces).
- Go-to-color and hotdog moves can go backward.
- Unclaimed cars can trigger the finish.
- A finish-triggering card's optional swap resolves before scoring.
- Turn order remains the entered name order; cards and car assignments randomize.
The supplied 'red go to blac swap' typo is treated as the former black,
now orange, car. Gray and grey both map to purple.

VALIDATION
Checked all 70 card actions, all die values, random assignment capacities for
all claim-limit boundaries, shared scoring, available-spot swaps, stars, negative
moves, finish handling, double points, undo, saved reload, and 20 complete
simulated three-round games with 15 players.

Additional checks cover forward/backward animation routes, control locking,
scoring after arrival, three-row space markup, and saved-game color migration.

Offline caching and readiness checks were verified with simulated network
failure. Physical iPad/Safari installation still needs a device test.
