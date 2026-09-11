# aotearoa_hansard_transcripts

A [morph.io](https://morph.io) scraper for NZ Parliament's per-day Hansard transcript pages,
which need a real browser (Radware's bot protection blocks plain HTTP requests) - that's the
only reason this is a separate scraper from
[aotearoa_hansard](https://github.com/Br3nda/aotearoa_hansard), which handles the Hansard search
API and sitting calendar without needing one.

**Data lives on morph.io, not in this repo**: <https://morph.io/Br3nda/aotearoa_hansard_transcripts>

That page has the scraper's run history and a `data.sqlite` you can query directly (via the page
itself, or morph.io's [API](https://morph.io/documentation/api)) - this repo is just the code
that produces it.

Downstream, [hotair](https://github.com/Br3nda/hotair) is what actually turns this (and
`aotearoa_hansard`'s) raw data into the structured, linked Debates/DebateItems/Members people
browse - this scraper only stores raw content, it doesn't parse anything itself.

**Status**: not built yet - still the default morph.io scraper template. See `aotearoa_hansard`'s
`PLAN.md` for where this fits into the overall plan.
