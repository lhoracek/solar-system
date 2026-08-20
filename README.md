# Solar System

Interactive 3D solar system visualization deployed at [solarsystem.lhoracek.cz](https://solarsystem.lhoracek.cz).

## Implementation

- The project is a single static page in `index.html`.
- Rendering is done with Three.js and OrbitControls loaded from CDNs.
- Planet, moon, and sun textures are generated procedurally with canvas drawing code instead of image assets.
- The scene models:
  - the Sun, planets, and selected moons
  - orbital motion with separate groups for orbital inclination and axial tilt
  - planetary rings for Saturn and Neptune
  - a generated starfield with a denser Milky Way band
- Interaction includes camera orbit controls, hover labels, click-to-follow targeting, and a time-scale slider.

## Deployment

- Production site: [https://solarsystem.lhoracek.cz](https://solarsystem.lhoracek.cz)
- The repository keeps the `CNAME` file because GitHub Pages uses it to bind the deployment to the custom domain `solarsystem.lhoracek.cz`.

## Local usage

Open `index.html` in a browser, or serve the repository root with any static HTTP server.
