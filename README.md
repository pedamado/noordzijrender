🧊 NoordzijRender: Deconstruct

A brutalist, web-based variable font inspector that dynamically deconstructs TrueType design spaces and renders interpolated instances across an interactive 3D Noordzij cube.

Inspired by the bold, modular aesthetics of Wim Crouwel, Karel Martens, and the heavy geometric graphics of Buro Destruct, NoordzijRender is an experimental typography tool designed for type design students, educators, and enthusiasts.

🚀 Features

Drag & Drop Parsing: Instantly load local Variable Fonts (.ttf) directly into the browser.

3D Design Space Projection: Maps up to 3 variation axes (e.g., Weight, Width, Optical Size) to the corners of an interactive 3D Gerrit Noordzij Cube.

Animated Ghost Interpolations: Visualizes the morphing paths between masters using transparent, overlapping sine-wave animations with independent cycling speeds.

Interactive Canvas: Click and drag to pan around the deconstructed typographic space.

Glyph Map Modal: Automatically caches and displays available glyphs with contours for quick character selection.

Deep Customization: A hidden brutalist drawer menu allows you to tweak overall font size, cube scale, depth (Z-axis shift), node radius, and master fill styles.

Vector Export: Export the exact rendered frame of the typographic cube to a clean, transparent SVG file.

Dark / Light Mode: Native responsive theming.

🛠 Under the Hood

Rendering variable fonts dynamically in HTML5 Canvas requires robust math. NoordzijRender relies on a dual-engine approach to guarantee precise point-by-point (IUP) interpolation:

OpenType.js: Handles base static parsing, metrics, cmap resolution, and fallback path generation.

Samsa-core.js: Acts as the primary TrueType (gvar / avar / fvar) parser, ensuring complex non-linear axes and sparse tuple coordinates interpolate flawlessly. The app intercepts Samsa's SVG paths and injects them back into the native canvas renderer.

💻 Usage

No build step is required. The app is a single, self-contained HTML file.

Clone the repository:

git clone [https://github.com/pedamado/noordzijrender.git](https://github.com/pedamado/noordzijrender.git)


Open index.html in any modern web browser.

Drag and drop a Variable Font (.ttf) onto the screen.

Open the + menu on the top right to access controls, toggle the animation, and export your compositions.

🎓 Credits & Context

Design & Direction: Pedro Amado (FBAUP/i2ADS).

Context: Developed within the context of the MDGPE Type Design Course and the Ligatures SIG from the i2ADS.

Development: Coded in collaboration with Gemini Pro (April 2026), showcasing the power of generative AI in rapid prototyping for bespoke typographic tools.

📄 License

This project is open-source. Feel free to fork, experiment, and deconstruct!
