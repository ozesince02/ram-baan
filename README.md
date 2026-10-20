<div align="center">

# राम बाण · RAM BAAN

**A five-minute pixel-art Dussehra quest.**
Five asuras. A road full of Maya. One bow, one prince, and one very flammable ten-headed effigy waiting at the end.

`single HTML file` · `zero dependencies` · `plays on desktop and phone` · `made for Vijayadashami`

**[▶ Play it in your browser](#play-it)**

</div>

---

## The story so far

Shri Ram has to walk from the forests of Dandaka, across the Ram Setu, to the golden gates of Lanka. Standing in the way: five asuras, and a road built by people who clearly hate you.

Beat an asura and you don't just walk on. A **Dharma Prashna**, a question of dharma written on a palm-leaf manuscript, appears. Answer well and the path opens. Answer badly and *adharma returns when wisdom falters*: the asura climbs back out of the smoke at full health and you go again.

Defeat all five, step through the gate, and the game hands you the remote. The finale is a cutscene: Ravan's arrogant speech, Ram's reply, the Brahmastra, and then the night of the mela, where three effigies go up in flames and fireworks.

## Play it

**Online:** <!-- PLAY_URL --> once GitHub Pages is switched on for this repo (Settings → Pages → Deploy from branch → `main` / root).

**Locally:** download `index.html` and double-click it. That's the whole game. No build, no install, no `node_modules` the size of Lanka.

If you'd rather serve it:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>.

## Controls

| Action | Keyboard | Phone |
| --- | --- | --- |
| Move | `←` `→` or `A` `D` | ◀ ▶ |
| Jump (hold for higher) | `Space`, `W` or `↑` | JUMP |
| Dash (brief invulnerability) | `Shift` or `L` | DASH |
| Shoot an arrow | `J`, `X` or click | BOW |
| **Divine arrow** (3× damage) | hold `J` until it sparkles, release | hold BOW |
| Answer a Dharma Prashna | `1` `2` `3` | tap |
| Pause / mute | `Esc` / `M` | top-right buttons |
| Full screen | FULL SCREEN button | FULL SCREEN button (Android; iPhones don't allow it) |

**On phones:** play in landscape. Hold your phone in portrait and the game pauses with a "turn your phone" screen. Rotate, and it picks up where you were. If you really want to, you can still tap *Play in portrait anyway*. Tablets get bigger buttons and work in either orientation.

Arrows home in on the asura you're facing, because Ram doesn't miss. You still have to survive long enough to let go of the string.

> **The one rule worth remembering:** jump the **white** (low) blades, dash through the **red** (high) ones.

## Rogues' gallery

| Asura | Who they are | What they'll do to you |
| --- | --- | --- |
| **Maricha** | The golden deer of Maya | Prances around looking innocent. Three arrows reveal the rakshasa underneath. |
| **Subahu** | Defiler of Vishwamitra's yagna | Rains fire from the sky. Watch the ground for the glowing shadows. |
| **Khara** | Fury of Janasthana | Throws knives in pairs and charges across the arena. Jump him or dash through him. |
| **Kumbhakarna** | The giant who slept six months | Starts asleep. Wake him with arrows (you will regret it). Ground-pound shockwaves, boulders, a club the size of a cow. |
| **Meghnad** | Indrajit, master of illusion | Flies on a storm cloud, vanishes, reappears, fires serpent arrows (nagpash) and dive-bombs you. |

## The road is lying to you

This is a troll game in the grand tradition of mobile pixel platformers. Every sign is a suspect.

<details>
<summary><b>Spoilers: the traps</b> (open only if you've died enough times to deserve it)</summary>

- **Pop-up spikes** that wait until exactly where you were going to land.
- A sign that says **SAFE GROUND AHEAD**, followed by ground that is not safe and, on closer inspection, not ground.
- **STEADY PLANKS.** They are not steady.
- A carved stone head that drops from the sky when you walk under it. Patience, Raghava.
- Boulders that roll in from behind, because asuras never fight fair.
- A sign that says **NOTHING SUSPICIOUS HERE**, then two spike traps timed against each other. Short hops win.
- **The Ram Setu.** Every stone carries the name राम and floats... except the three that sink. Makara fish leap through the gaps.
- **Lanka's fire jets**, a timing puzzle in gold.
- A **checkpoint diya** that isn't a checkpoint.
- Gold floors that drop away, because Ravan's builders cut corners.
- A final sign: **RAVAN'S GATE. DEFINITELY NO TRAPS.** (It's telling the truth. We felt that you'd earned it.)

</details>

Every death brings a short message, from *"Only stones with Ram's name float. You are not a stone."* to *"Rolling stones gather no dharma."* Checkpoint diyas light up along the way, so you'll never lose much progress.

## What the questions teach

The ten Dharma Prashnas come straight from the Ramayana, each paired with the asura you just beat:

- **The golden deer:** glittering temptations pull us away from dharma.
- **The Lakshman Rekha:** limits drawn for our safety deserve respect.
- **Guarding the yagna:** strength exists to protect the good and the helpless.
- **Shabari's berries:** sincere devotion matters more than status or ritual.
- **Fourteen years of exile:** *praan jaaye par vachan na jaaye*. A promise kept is dharma.
- **Bharat and the padukas:** selfless love over personal power.
- **Vibhishan's choice:** truth over blind loyalty.
- **Indrasan vs Nidrasan:** think before you speak, because words carry power.
- **The squirrel on the Setu:** no effort is too small when it is sincere.
- **Ravan's ten heads:** kaam, krodh, moh, lobh, mad, matsar, swarth, anyaay, amanavta, ahankaar. The real Ravan to burn is the one inside.

## The finale

1. Ram walks through the gate into blinding light.
2. Thunder. Ravan rises out of the battlefield, one head at a time. All ten.
3. *"Kneel, Raghava. In all three worlds there is no one greater than Ravan!"*
4. Ram's answer: *"Ten heads of knowledge, and not one of them learned humility."*
5. The Brahmastra charges, the screen goes gold, and the arrow finds its mark.
6. Cut to a night-time Dussehra mela: string lights, a Ferris wheel, a crowd with phones in the air, and the three putlas of **Meghnad, Ravan and Kumbhakarna**.
7. A flaming arrow. Fire climbs from the hem to the crown. Ravan's heads burst one by one as fireworks. *Asatya par satya ki vijay.*

At the end you get your time, your deaths and how many questions you got right. Compare with friends. Lie about the deaths.

## How it's made

Everything lives in one file, [`index.html`](index.html). No engine, no framework, no image assets, no audio files.

- **Pixel rendering.** The game draws to a 384 × 216 canvas and scales it up with nearest-neighbour filtering. Every character, from Ram's crown to Kumbhakarna's belly, is drawn rectangle by rectangle in code.
- **Fake bloom.** Glowing things (diya flames, divine arrows, fireballs, fireworks) are also painted onto a separate glow layer. That layer is shrunk to a quarter size, stretched back with smoothing on, and added on top, which gives a cheap, soft glow.
- **A 3 × 5 bitmap font** for in-game text, defined as 15-bit strings, so signs and boss names stay crisp at any size.
- **Generated sound.** Web Audio synthesizes every sound live: dhol beats (pitch-dropping sine plus noise), tanpura plucks cycling Pa–Sa–Sa–Sa, and a shehnai-style lead (a vibrato sawtooth through a bandpass filter) playing pentatonic or Bhairav-flavoured phrases. Music changes with the moment: calm in the fields, frantic in boss fights, festive at the mela.
- **The effigies** are painted into their own off-screen canvases each frame. A gradient composited with `source-atop` chars them from the bottom up as they burn.
- **Game feel:** coyote time, jump buffering, variable jump height, i-frame dashes with afterimages, hit-stop, screen shake, and a ledge step-up so near-misses count.
- **Fonts:** Press Start 2P, Pixelify Sans and Tiro Devanagari Hindi from Google Fonts. Everything else is hand-made.

## Project layout

```
ram-baan/
├── index.html   # the entire game
├── README.md    # you are here
└── .gitignore
```

## Ideas for next Dussehra

- A Hanuman level: leap across the ocean, set Lanka's rooftops on fire.
- Hindi language toggle for the questions and dialogue.
- A speedrun timer with split times per asura.
- Lakshman as a second player.

PRs welcome. Ravan-themed PRs will be reviewed with suspicion.

---

<div align="center">

**शुभ विजयादशमी!** May the only thing you burn this year be your own ego (and maybe a little popcorn at the mela).

*Jai Shri Ram.*

</div>
