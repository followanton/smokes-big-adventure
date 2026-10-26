# Smoke's Big Adventure

A 3D story game in the browser. Dr. Doge's robot dogs have taken over Neo-Paw City, a neon cyber city. Smoke the cat, with help from Bolt the hacker mouse, has to stop them.

## Play

Double-click `index.html` to open it in a web browser. It needs an internet connection, because it loads the 3D engine (three.js) from the web. Your chapter progress is saved in the browser, so you can pick up where you left off.

Online: **https://smokes-grote-avontuur.onrender.com**

- It's a free Render static site, built from this repository's `main` branch.
- Every push to `main` puts the new version online within about a minute.
- Coins and progress are saved per website, so the online game keeps its own.

## Languages

The game is in Dutch (*Smokes Grote Avontuur*), and English is kept alongside it.

- Every text the player sees is in one table, `T`, at the top of `index.html`, with an `en` and an `nl` version side by side. The story lines and the chapter names sit in `CHAPTERS`, `HIDEOUT` and `ENDING` as `{ en, nl }` pairs.
- `let lang = 'nl'` picks the language. Until there is a language switch, change it to `'en'` for English.
- The words on signs, billboards and screens in the city are drawn when the game starts, so a language switch should reload the page.
- Dutch texts are kept no longer than the English ones, so no button or box overflows.
- The names stay the same in both languages: Smoke, Bolt, Dr. Doge, Neo-Paw City and the robots (Pup-Bot, Dash-Bot, Tank-Bot, Zap-Hound, Mega-Hound). In Dutch a chapter is called a "level".

## Coins and outfits

Every star Smoke earns is also a 🪙 coin. Coins are saved in the browser and stay when you start a new game or lose in Hardcore. Spend them in 🎩 Outfits on the main menu, where Smoke shows off each hat up close. Buy a hat once, then wear it (or take it off) whenever you like. It shows in the levels and the movies too.

| Outfit | Coins |
|---|---|
| 🎉 Party Hat | 500 |
| 🎩 Top Hat | 1,000 |
| 😎 Cool Shades | 1,500 |
| 🤠 Cowboy Hat | 2,000 |
| 🏴‍☠️ Pirate Hat | 3,000 |
| 🐶 Doggy Hat | 4,000 |
| 🧙 Wizard Hat | 5,000 |
| 👑 Crown | 7,500 |
| 🤖 Robot Dog Helmet | 8,000 |
| 🐟 Fish Hat (a giant fish eating Smoke's head) | 10,000 |

## Controls

- W A S D or arrow keys: run. Shift: sprint (uses the blue bar).
- F, J or a mouse click: claw slash. It also knocks lasers away.
- Space: jump. Robots can't climb crates.
- Drag the mouse, or Q and E: turn the camera. Mouse wheel: zoom.
- Hide in the glowing holo-bushes, but not with a robot right behind you.
- M: open the big map (the game waits while it is open). P or Esc: pause.

All of these keys can be changed in ⚙️ Settings (on the main menu and the pause screen). Settings also turns the music and the sound effects on or off. Your choices are saved in the browser.

## Graphics

Neo-Paw City is a rainy neon city: wet streets with puddles that reflect the lights, glowing shop windows and signs, moving billboards, steam, and a skyline with Doge Tower in the distance. Street lamps really light up Smoke and the robots as they pass.

The buildings come in three styles: office towers (rows of windows between stone columns), shiny glass skyscrapers (small panes in thin metal frames that reflect the city), and apartments (bigger windows with balconies, curtains and air conditioners). Tall towers get a stepped top, a pointy crown with a spire, or a water tower.

Settings has a Graphics switch. High has the puddle reflections, more rain and sharper shadows. Low runs faster on older computers. If the game runs slowly, it switches to Low by itself once, unless you picked a setting yourself.

## Music

Every chapter has its own song, and the main menu has one too. The game makes the music itself while you play, so there are no music files. The music goes quieter while the game is paused or the map is open.

## Modes

New story asks which mode to play:

- 🙂 Normal: if the robots catch Smoke, you try that chapter again.
- 💀 Hardcore: if the robots catch Smoke even once, you go back to Chapter 1 and your stars go back to 0. Hardcore doesn't save your chapter, so you have to beat the whole game in one go. Beat it and the ending says you are a true champion.

## Story movies

The story is told in little animated movies before each chapter, with the words shown as subtitles. Click or press Space to go on faster, and Esc or the Skip button skips the movie.

- Before chapter 1: Smoke naps on a rooftop, Dr. Doge appears as a giant hologram in the sky, and Bolt pops out of a manhole.
- After chapter 1: Bolt opens the manhole at the blue beam, and Smoke follows him down into his secret sewer hideout (green water, pipes, Bolt's computers and a spinning Dash-Bot hologram).
- The other chapters: a flight past the generators, a Zap-Hound firing its laser, a parade of every kind of robot dog, the Mega-Hound's roar, and a happy ending.

## Chapters

1. Neon Streets: reach Bolt's hideout.
2. Training Day: defeat 3 robot dogs.
3. Power Down: smash 3 generators.
4. Laser Alley: reach Doge Tower.
5. The Big Blackout: smash 4 generators.
6. Mega-Hound: beat the boss.

## Robot dogs

| Robot | Looks | What it does |
|---|---|---|
| Pup-Bot | grey, blue eyes | the basic robot dog, 2 hits |
| Dash-Bot | yellow | fast (sprint to get away), 1 hit |
| Tank-Bot | red, big | slow, 4 hits, bites for 2 hearts |
| Zap-Hound | purple, cannon | keeps its distance, flashes its eyes, shoots a laser a little ahead of you |
| MEGA-HOUND | huge boss | charges when its eyes glow, shoots laser fans, calls backup. Crashes into walls and gets dizzy (double damage). |

The robot dogs are smart. They run to where Smoke is going, come at Smoke from the sides, and bark to call the dogs nearby. When they lose Smoke, they look where Smoke was heading and sometimes sniff the closest holo-bush. If Smoke is on a crate, they circle it and wait. Dash-Bots bite and then run off.

Smoke has 5 hearts. Fish snacks heal 1 heart.

Everything is in `index.html`.
