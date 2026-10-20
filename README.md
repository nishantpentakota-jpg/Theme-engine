# Image-Based Theming Engine

Upload a wallpaper, extract its colors, and generate a live UI theme.
Built by <Your Name> for E-Cell NITK Technical Recruitments 2026 (Task 3).

## How it works
- **Color extraction:** Color Thief reads the image pixels and returns the 6 dominant colors, shown as clickable swatches.
- **Theme generation:** The user picks which swatch becomes Primary, Secondary, Background, or Card color. All choices are stored in one state object, and a single `render()` function writes them as CSS variables.
- **Consistency:** Every UI component reads only from those CSS variables, so one change updates the whole preview.
- **Presets:** Minimal, Vibrant, Warm, Cool, and Glass each change background, card style, corner radius, shadow, saturation, and blur.
- **Adjustments:** Saturation, brightness, contrast, background blur, and overlay opacity sliders update the preview in real time.
- **Accessibility:** Text color is chosen automatically (black or white) based on the luminance of the background, so text stays readable.
- **Responsive:** CSS grid layout stacks on screens narrower than 800px.

## Design decisions
- Plain HTML, CSS, and JavaScript with no build step, so it runs by opening `index.html`.
- One render function as the single source of truth for the theme.
- Smooth CSS transitions when themes change.

## Run it
Open `index.html` in any browser.

## Note
I used AI assistance (Claude) to help me learn and build this project, and I customized and tested it myself.# Theme-engine
