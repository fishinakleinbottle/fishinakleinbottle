## Hi, I'm Sreeram

I lead the engineering team and build technology at [Noora Health](https://www.noorahealth.org), where we train family
caregivers across India and Bangladesh. In practice that means a lot of WhatsApp infrastructure
and a lot of content tooling.

I'm also co-building [CommonerLLP](https://commonerllp.org), where we make tools for reading
the Indian state's own paperwork: parliamentary questions, committee reports, budget documents,
public university hiring. The work turns scattered records into public knowledge you can find and
cite, like [theright2read.org](https://theright2read.org) and
[whoseuniversity.org](https://whoseuniversity.org).

Some of my work sits under
[@noorahealthtech](https://github.com/noorahealthtech), my Noora Health account, rather than this
one.

## What I've contributed to

**[Understand-Anything](https://github.com/Egonex-AI/Understand-Anything)** turns a codebase into a
knowledge graph you can explore and ask questions about. I swapped its hardcoded TypeScript
assumptions for a language and framework registry — 12 languages, 10 frameworks — rebuilt the
dashboard navigation around architectural layers, and fixed a bug where parallel analyzer runs
produced mismatched node IDs and quietly dropped edges.

**[context-hub](https://github.com/andrewyng/context-hub)** is a library of documentation written
for LLMs rather than for people. I wrote the Ruby and Rails coverage: ActiveRecord,
ActionController, ActiveJob, Devise, Sidekiq, RSpec, FactoryBot, Faraday, and HTTParty.

**[courier](https://github.com/nyaruka/courier)** is the messaging gateway behind
[RapidPro](https://rapidpro.io) and [TextIt](https://textit.com), and what our WhatsApp traffic runs
through at Noora Health, via [Turn](https://www.turn.io). I fixed the Turn handler dropping header,
button, and media components from outgoing templates, and made its 429s retry as throttled rather
than fail. Shipped in v26.3.x, authored from [@noorahealthtech](https://github.com/noorahealthtech).

**[parliamentwatch](https://github.com/pranaykotas/parliamentwatch)** tracks Indian Parliamentary
Committee reports from sansad.in. I added the rosters that were previously buried in report PDFs:
490 members across all 16 standing committees, matched against the Lok Sabha and Rajya Sabha
directories and linked to their sansad.in biographies.

## What I've built

**[commoner-probe](https://github.com/CommonerLLP/commoner-probe)** handles acquisition for
everything we build at CommonerLLP. Public disclosures sit on undocumented portals with no bulk
export and PDFs you can't read programmatically. This deals with that part so the analysis code
doesn't have to.


**[dots-mcp](https://github.com/noorahealthtech/dots-mcp)** puts [DOTS](https://getdots.in/), the
knowledge platform we use at Noora Health, behind a chat interface using
[MCP](https://modelcontextprotocol.io). The model gets a set of retrieval tools and decides what to
search for itself, so the whole knowledge base never has to fit in the context window. It runs in
mock mode without credentials, which means you can wire it into Claude and watch the tool calls
work before you have a token. Built under
[@noorahealthtech](https://github.com/noorahealthtech).

## Also working on

A fair amount of what I spend time on is in private repos

- A rehearsal tool for theatre companies. Script parsing across several formats, annotation, and
  practice sessions with text-to-speech.
- A [Spanish learning platform](https://plaza.aventurahispana.com/)
