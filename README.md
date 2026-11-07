# 23 home pages

Twenty-three different home pages for the same content: a title and four projects. Pick one, replace the title, the projects and the icons, and it is yours.
They are numbered 01–24, and 08 is missing: it is kept for the author's own site.

<table>
  <tr>
    <td align="center" valign="top"><a href="templates/01-manifesto.html"><img src="assets/screenshots/01-manifesto.png" width="220" alt="01 manifesto"></a><br><b>01</b> manifesto</td>
    <td align="center" valign="top"><a href="templates/02-risograph.html"><img src="assets/screenshots/02-risograph.png" width="220" alt="02 risograph"></a><br><b>02</b> risograph</td>
    <td align="center" valign="top"><a href="templates/03-bauhaus.html"><img src="assets/screenshots/03-bauhaus.png" width="220" alt="03 bauhaus"></a><br><b>03</b> bauhaus</td>
    <td align="center" valign="top"><a href="templates/04-paper.html"><img src="assets/screenshots/04-paper.png" width="220" alt="04 paper"></a><br><b>04</b> paper</td>
  </tr>
  <tr>
    <td align="center" valign="top"><a href="templates/05-aurora.html"><img src="assets/screenshots/05-aurora.png" width="220" alt="05 aurora"></a><br><b>05</b> aurora</td>
    <td align="center" valign="top"><a href="templates/06-warm-grain.html"><img src="assets/screenshots/06-warm-grain.png" width="220" alt="06 warm grain"></a><br><b>06</b> warm grain</td>
    <td align="center" valign="top"><a href="templates/07-liquid.html"><img src="assets/screenshots/07-liquid.png" width="220" alt="07 liquid"></a><br><b>07</b> liquid</td>
    <td align="center" valign="top"><a href="templates/09-liquid-chrome.html"><img src="assets/screenshots/09-liquid-chrome.png" width="220" alt="09 liquid chrome"></a><br><b>09</b> liquid chrome</td>
  </tr>
  <tr>
    <td align="center" valign="top"><a href="templates/10-brushed-aluminium.html"><img src="assets/screenshots/10-brushed-aluminium.png" width="220" alt="10 brushed aluminium"></a><br><b>10</b> brushed aluminium</td>
    <td align="center" valign="top"><a href="templates/11-brass.html"><img src="assets/screenshots/11-brass.png" width="220" alt="11 brass"></a><br><b>11</b> brass</td>
    <td align="center" valign="top"><a href="templates/12-chrome-title.html"><img src="assets/screenshots/12-chrome-title.png" width="220" alt="12 chrome title"></a><br><b>12</b> chrome title</td>
    <td align="center" valign="top"><a href="templates/13-neon-signs.html"><img src="assets/screenshots/13-neon-signs.png" width="220" alt="13 neon signs"></a><br><b>13</b> neon signs</td>
  </tr>
  <tr>
    <td align="center" valign="top"><a href="templates/14-holographic.html"><img src="assets/screenshots/14-holographic.png" width="220" alt="14 holographic"></a><br><b>14</b> holographic</td>
    <td align="center" valign="top"><a href="templates/15-frosted-glass.html"><img src="assets/screenshots/15-frosted-glass.png" width="220" alt="15 frosted glass"></a><br><b>15</b> frosted glass</td>
    <td align="center" valign="top"><a href="templates/16-oscilloscope.html"><img src="assets/screenshots/16-oscilloscope.png" width="220" alt="16 oscilloscope"></a><br><b>16</b> oscilloscope</td>
    <td align="center" valign="top"><a href="templates/17-terminal.html"><img src="assets/screenshots/17-terminal.png" width="220" alt="17 terminal"></a><br><b>17</b> terminal</td>
  </tr>
  <tr>
    <td align="center" valign="top"><a href="templates/18-led-matrix.html"><img src="assets/screenshots/18-led-matrix.png" width="220" alt="18 LED matrix"></a><br><b>18</b> LED matrix</td>
    <td align="center" valign="top"><a href="templates/19-split-flap.html"><img src="assets/screenshots/19-split-flap.png" width="220" alt="19 split-flap"></a><br><b>19</b> split-flap</td>
    <td align="center" valign="top"><a href="templates/20-teletext.html"><img src="assets/screenshots/20-teletext.png" width="220" alt="20 teletext"></a><br><b>20</b> teletext</td>
    <td align="center" valign="top"><a href="templates/21-objects.html"><img src="assets/screenshots/21-objects.png" width="220" alt="21 objects"></a><br><b>21</b> objects</td>
  </tr>
  <tr>
    <td align="center" valign="top"><a href="templates/22-diorama.html"><img src="assets/screenshots/22-diorama.png" width="220" alt="22 diorama"></a><br><b>22</b> diorama</td>
    <td align="center" valign="top"><a href="templates/23-particles.html"><img src="assets/screenshots/23-particles.png" width="220" alt="23 particles"></a><br><b>23</b> particles</td>
    <td align="center" valign="top"><a href="templates/24-acrylic.html"><img src="assets/screenshots/24-acrylic.png" width="220" alt="24 acrylic"></a><br><b>24</b> acrylic</td>
  </tr>
</table>

Each page is a single HTML file (CSS and JavaScript inside, no build step), designed for a phone in portrait. The designs were drawn by
Claude Opus 5.5 for Federico Anastasi's website; they are cleaned up here and neutral, ready to be taken and adapted. MIT licence.

## How to use

1. Serve the folder with any static server (see below) and open `index.html`: it shows the 23 pages inside a phone, with number, name and a link to open each one.
2. Pick the one you like and copy its file from `templates/` into your project, together with the `assets/` folder
   (paths are relative: `templates/` and `assets/` must stay next to each other, or update the `../assets/` paths).
3. Open the file: the comment at the top ("HOW TO USE") says where the title, the projects and the icons are in that page.
4. Replace:
   - the title: "Your open space" and "by First Last";
   - the four projects: "Project one ... four", the line "a short line" and the category;
   - the icons: `assets/project-1.svg ... project-4.svg` (square, transparent background: you can keep the same names);
   - the links `#project-1 ... #project-4`, with the addresses of your own projects.

In some pages the text is not only in the HTML but also in the script, because it is drawn on a canvas or on a 3D texture
(12, 16, 18, 19, 20, 23) or typed by an animated demo (17): the comment at the top of the file says where.

### Local server

The 3D pages load images into WebGL and do not work when opened by double-clicking the file (`file://`).
Any static server will do; from the repo folder:

```
python -m http.server 8000
```

then open `http://127.0.0.1:8000/`.

## Libraries and external resources

An internet connection is needed the first time a page loads.

- **Fonts**: every page loads a font from Google Fonts (with a system fallback if it does not load).
- **three.js r128** from cdnjs: `12-chrome-title`, `21-objects`, `22-diorama`, `23-particles`, `24-acrylic`.
- The other pages use no libraries: only CSS, SVG, 2D canvas, or hand-written WebGL (`05-aurora`, `09-liquid-chrome`, `15-frosted-glass`).

To use them offline, download the fonts and `three.min.js` and change the addresses in the files.

## The pages

| no. | name | idea |
|-----|------|------|
| 01 | [manifesto](templates/01-manifesto.html) | Swiss-style layout, huge title, a red rule that draws itself |
| 02 | [risograph](templates/02-risograph.html) | three-ink print, overlapping shapes slightly out of register |
| 03 | [bauhaus](templates/03-bauhaus.html) | flat shapes and primary colours |
| 04 | [paper](templates/04-paper.html) | layered cut paper with real-thickness shadows |
| 05 | [aurora](templates/05-aurora.html) | a warm gradient that slowly flows, in WebGL |
| 06 | [warm grain](templates/06-warm-grain.html) | bands of light with film grain |
| 07 | [liquid](templates/07-liquid.html) | four drops that merge and separate again |
| 09 | [liquid chrome](templates/09-liquid-chrome.html) | chrome drops whose reflection follows your finger |
| 10 | [brushed aluminium](templates/10-brushed-aluminium.html) | brushed aluminium plates |
| 11 | [brass](templates/11-brass.html) | enamelled brass plaques with push buttons |
| 12 | [chrome title](templates/12-chrome-title.html) | a 3D chrome title and four metal tokens (three.js) |
| 13 | [neon signs](templates/13-neon-signs.html) | neon signs on a brick wall |
| 14 | [holographic](templates/14-holographic.html) | embossed holographic seals |
| 15 | [frosted glass](templates/15-frosted-glass.html) | slabs of frosted glass |
| 16 | [oscilloscope](templates/16-oscilloscope.html) | amber-phosphor Lissajous figures |
| 17 | [terminal](templates/17-terminal.html) | a terminal with four live processes |
| 18 | [LED matrix](templates/18-led-matrix.html) | a dot-matrix LED panel |
| 19 | [split-flap](templates/19-split-flap.html) | a split-flap departures board, as in a railway station |
| 20 | [teletext](templates/20-teletext.html) | a teletext page behind a TV-set glass |
| 21 | [objects](templates/21-objects.html) | four glossy 3D objects (three.js) |
| 22 | [diorama](templates/22-diorama.html) | an isometric 3D room (three.js) |
| 23 | [particles](templates/23-particles.html) | thirty thousand points of light that form the title (three.js) |
| 24 | [acrylic](templates/24-acrylic.html) | acrylic slabs that catch the light (three.js) |

## Licence

MIT, see `LICENSE`.
