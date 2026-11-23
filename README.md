# Goblin Grab

A location-based creature-catching game, as suggested by Greg: there's only one kind of creature (a goblin), and about **1 in every 1000 is yellow**.

## Play

Open `index.html` in a browser. It needs an internet connection for the map tiles. The map uses Esri's World Street Map tiles, which need no API key. OSM's own tile servers block pages opened from a local file, and CARTO's need an API key.

- **Use my real location**: walk around in real life. Goblins spawn around you. Tap one when it's inside your yellow circle (70 m).
- **Demo mode**: walk with WASD or the arrow keys (hold Shift to run), or use the on-screen D-pad.

In an encounter, flick the sack upward at the goblin. Throw while the shrinking ring is small for a better chance (Nice / Great / Excellent). Goblins can break out of the sack, and some run away. Yellow goblins move faster, are harder to bag, and run away more often.

When you run low on sacks, tap a goblin den (the stick huts) to get more. Each den restocks after 2.5 minutes.

Your **Ledger** saves every goblin you catch in browser localStorage.

## Playing on a phone

Phones only give location to pages served over HTTPS. Put the file on any static host (GitHub Pages, Netlify Drop, etc.) and open that URL on your phone.

## Testing the yellow goblin

Add `?yellow` to the URL (`index.html?yellow`) to make half of all goblins yellow.
