# Wardley mapping workshop · DDD Belgium · 20 October 2026

The slide deck, the maps and the reading list for the Wardley mapping workshop at DDD Belgium,
given by Christian (CJ) Johansen, GalaxiTech. The evening runs as teach, group exercise, discussion,
six times, around one fictional company, Harbour Insurance.

## What is here

| Path | What it is |
| --- | --- |
| `workspaces/ddd-belgium-wardley/ddd-belgium-wardley.md` | The deck, a Marp markdown file. `ddd-belgium-wardley.html` is the built version: open it in a browser |
| `workspaces/ddd-belgium-wardley/diagrams/*.mmd` | Every map as Mermaid `wardley-beta` source, one file per map |
| `workspaces/ddd-belgium-wardley/assets/diagrams/*.svg` | The rendered maps |
| `workspaces/ddd-belgium-wardley/workshop-plan.md` | The plan: the company, the storyline through the six exercises, timings |
| `workspaces/ddd-belgium-wardley/wardley-sources.md` | The reading list: the books that use Wardley maps, with page references and one redrawn map per book |
| `workspaces/ddd-belgium-wardley/schon-annex-maps.md` | Erik Schön's annex of 168 Wardley maps, indexed by mapper |
| `workspaces/ddd-belgium-wardley/assets/wardley/` | Simon Wardley's own figures used on the slides, with `SOURCES.md` |
| `workspaces/ddd-belgium-wardley/assets/books/` | The book covers, from the publishers' and authors' own pages, with `SOURCES.md` |
| `themes/galaxitech.css`, `scripts/` | The Marp theme, the map renderer, the reveal generator and the slide validator |

## Rebuild it

Needs Node 20 or newer and a local Chrome (set `CHROME_PATH` if it is not in the default place).

```bash
npm install
npm run ddd
```

That regenerates the reveal maps, renders every map to SVG, validates the deck (overflow, overlaps,
unknown classes) and builds the HTML. `npm run dev` serves the deck on http://localhost:8080.

## Credits and licences

- Simon Wardley's figures (`assets/wardley/`) are from his book *Wardley Maps*, CC BY-SA 4.0, taken
  from the community copy at github.com/andrewharmellaw/wardley-maps-book. They are shown as he
  drew them. Maps marked "after Simon Wardley" are redrawn from his CC BY-SA figures and carry the
  same licence.
- Maps marked "after" another author (`diagrams/book-*.mmd`) are redrawn from one figure in that
  author's book, with the figure and page named on the map. Where the book is all rights reserved the author was asked first; the maps whose
  authors have not answered yet are held back from this copy. See `wardley-sources.md` for the figure each
  one follows and where a line is a judgement.
- The Wardley Mapping Canvas is by Ben Mosior, CC BY-SA 4.0. Photos are credited on the slide
  that shows them.
- The GalaxiTech Display typeface is Montserrat (SIL Open Font License) with two altered capitals;
  the other fonts are from Fontsource, also under the SIL Open Font License.
- Everything else, the slides, the text, the Harbour Insurance scenario and our own maps, is by
  Christian Johansen, GalaxiTech, and released under the same licence, CC BY-SA 4.0 (see `LICENSE`).
  Reuse it with credit, and share what you build on it under the same terms.
