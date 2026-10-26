# AI Sluggers Baseball

A browser baseball game featuring animal all-stars, super-powered pitches and swings, and three-inning matches. Every at-bat starts with one ball and one strike. Choose Home (pitch first, bat second) or Away (bat first, pitch second) before starting.

## Play locally

Open `index.html` in a browser, or run `python -m http.server 8000` from this directory. No build step or dependencies are required.

## Controls

- Bat: Space, tap the field, or Swing.
- Pitch: aim with pointer or arrow keys, choose 1–3, then Space or Throw.
- Super: E when the meter is full, before a pitch.
- Pause: P or Escape.
- Sound: toggle synthesized arcade effects.

## Publish with GitHub Pages

In this repository, open Settings → Pages. Choose **Deploy from a branch**, then **main** and **/ (root)**, and Save. After deployment, the game will be available at https://jakestark1.github.io/AI-Sluggers-Baseball/ .

## Super powers and contact

Activation randomly chooses Fire/Thunder/Meteor Bat or Ghost/Tornado/Frost Ball. The powers in each group share outcome odds and have themed screen effects: flames, lightning, meteors, ghosts, tornadoes, or snowflakes. Reduced-motion preferences replace moving effects with a soft glow and power label. Powered pitches home into the zone. Pitching power takes precedence if both sides activate powers on the same pitch. A batting power is consumed on the swing.

A ball completely outside the strike-zone rectangle, including its 21-pixel plate radius, always produces a swing and miss. A ball touching an edge remains hittable. This rule applies to both batters and overrides batting powers.

Normal pitches released in the accuracy meter’s red sections drift more than green-section releases. Pitches touching any edge of the zone count as strikes when taken; fully outside pitches count as balls when taken and strikes when swung at.
