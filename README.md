# The Museum of AI Safety

A first-person, walkable museum in a single HTML file. No dependencies, no build step,
no network — a software-rendered raycasting engine (the *Wolfenstein 3D* technique),
procedural textures, synthesized WebAudio ambience, and 23 curated exhibits on AI safety.

## Run it

Open `index.html` directly in a browser, or serve it:

```sh
python3 -m http.server 8777
# → http://localhost:8777
```

## Controls

| Key | Action |
| --- | --- |
| `W A S D` / `↑ ↓` | walk |
| Mouse (click to capture) / `← →` | look |
| `E` / `Enter` / click | view exhibit |
| `Shift` | brisk pace |
| `M` | floor plan |
| `N` | sound on/off |
| `V` | audio guide (while reading a placard) |
| `G` | museum directory — click any exhibit to be escorted there |
| `J` | the Gift Shop — volunteer, learn, join the field |
| `H` | help · `0` in help resets your tour |
| `← →` | previous / next exhibit (while reading a placard) |

On phones: left thumb walks, right thumb looks, tap to open exhibits.

## The floor plan

Eight halls, 34 exhibits — the Foyer, the Gallery of Failures (adversarial examples,
jailbreaks, shortcut learning, sycophancy), the Rotunda with four governance pillars
under a skylight, Origins Hall (Wiener, Turing, Good, the paperclip era), the Glass
Brain (interpretability), and the Genie Room (alignment) — plus two newer wings:

- **The Old Office** (off the Foyer, west): a period diorama of the pre-AI workplace
  sealed behind a floor-to-ceiling **glass vitrine** — five 3D desks with seated
  workers, a water-cooler conversation, a filing cabinet, a photocopier (billboard
  sprites, z-buffered behind the pane). Placards and the gilt-framed oils hang in the
  viewing gallery on your side of the glass. Warm sepia light, typewriter clatter.
- **The Hall of Forecasts** (through the Genie Room, east): AGI timelines as a live
  split-flap **departures board** — Turing 2000, Simon 1985, Minsky DELAYED, Metaculus
  UPDATING LIVE, and a final row: YOU · BOARDING. Exhibits on scaling laws, the
  superforecaster tournament, takeoff speeds, and the No Fire Alarm pillar you must
  walk around. Cool blue light, a clock ticking once per second.

Origins Hall carries *The March of Progress (Amended)* — a five-block mural of the
evolution from ape to desk worker to phone-sloucher to robot to AI orb — protected,
like the office, behind brass-framed museum glass (rays pass through the pane with a
sliding specular streak; exhibits remain readable and clickable through it).

Every hall now displays its placards' artifacts as **3D pedestals under glass
domes** — the boat-race trophy, the paperclip, the gilt mirror, the GPU on its
cushion, the glass neuron, the fire-alarm-with-no-bell hourglass and ramps, the
empty pedestal of the finale — eighteen in all, placed at gallery angles. The
directory escort now drops you at a three-quarter view, museum-catalog style.

Behind the title wall, two doors open into **The Gift Shop · Get Involved**: a real
room with browsable shelf aisles. Every shelf is a product (BlueDot, Apart, 80,000
Hours, MATS, …) — walk up, press E, and "take it" opens the real link. **GET INVOLVED
vending machines** flank the doors: glass front, coiled product packs, a coin slot
labeled INSERT ATTENTION — press E to open the catalog.

The museum's name appears twice: as large extruded-gold 3D letters floating and
bobbing in the air of the Foyer, and as a perspective-tilted 3D masthead fixed at
the top of the screen everywhere (click it to return to the Foyer). The finale,
Exhibit Nº 35, stands in the center of the Rotunda.

Two **Gift Shop kiosks** flank the exit: real links to volunteer, study, and work in
AI safety (BlueDot, AISafety.info, Apart Research, AI Safety Camp, 80,000 Hours, MATS,
GovAI, and more). Also reachable any time with `J` or the on-screen buttons.

Progress persists in `localStorage`. See all 35 exhibits for your certificate.
Rendering resolution auto-tunes to hold 60 fps on your machine.

The map is a grid of text — edit `MAPSTR` in `index.html` to renovate the building;
add a letter and a matching entry in `EXHIBITS` to donate a new exhibit.
