## Hi, I'm Sreeram

I build technology at [Noora Health](https://www.noorahealth.org), where we train family
caregivers across India and Bangladesh. In practice that means a lot of WhatsApp infrastructure
and a lot of content tooling.

I'm also co-building [CommonerLLP](https://commonerllp.github.io), where we make tools for reading
the Indian state's own paperwork: parliamentary questions, committee reports, budget documents,
public university hiring. All of it is technically public. Almost none of it is usable. We build
the things that make it usable, like [theright2read.org](https://theright2read.org) and
[whoseuniversity.org](https://whoseuniversity.org).

Some of my work sits under
[@noorahealthtech](https://github.com/noorahealthtech), my Noora Health account, rather than this
one.

## What I've contributed to

**[Understand-Anything](https://github.com/Egonex-AI/Understand-Anything)** turns a codebase into
a knowledge graph you can explore and ask questions about.

It used to assume everything was TypeScript. I replaced the hardcoded parts with a language and
framework registry, so it now covers 12 languages and 10 frameworks, and adding another one means
writing a config file instead of editing if-blocks. I also rebuilt the dashboard navigation around
architectural layers, since a flat graph of a large repo is unreadable, and tracked down a bug
where parallel analyzer runs produced mismatched node IDs and quietly dropped edges.

**[context-hub](https://github.com/andrewyng/context-hub)** is a library of documentation written
for LLMs rather than for people.

I wrote the Ruby and Rails coverage: ActiveRecord, ActionController, ActiveJob, Devise, Sidekiq,
RSpec, FactoryBot, Faraday, and HTTParty. Each one is a short entry point with reference files
underneath, so an agent reads the overview first and pulls detail only when it needs it.

**[courier](https://github.com/nyaruka/courier)** is the messaging gateway behind
[RapidPro](https://rapidpro.io) and [TextIt](https://textit.com). It's also what our WhatsApp
traffic runs through at Noora Health, via [Turn](https://www.turn.io).

The Turn handler only built `body` components when it sent a template, so anything in the header
or the buttons got dropped on the way out. Media templates looked like they sent fine and arrived
with no image. Worse, a template that also carried attachments took a different branch entirely
and never sent the template at all. I fixed both, and made Turn's 429s retry as throttled instead
of failing permanently. Shipped in v26.3.x, and authored from
[@noorahealthtech](https://github.com/noorahealthtech).

**[parliamentwatch](https://github.com/pranaykotas/parliamentwatch)** tracks Indian Parliamentary
Committee reports from sansad.in.

If you wanted to know who actually sits on a committee, you had to dig through report PDFs. I
pulled the rosters properly instead: 490 members across all 16 standing committees, matched
against the Lok Sabha and Rajya Sabha directories, each one linked to their sansad.in biography.

## What I've built

**[commoner-probe](https://github.com/CommonerLLP/commoner-probe)** handles acquisition for
everything we build at CommonerLLP. Public disclosures sit on undocumented portals with no bulk
export and PDFs you can't read programmatically. This deals with that part so the analysis code
doesn't have to.

I added the Union Budget, bills, floor debates, and academia sources, along with parsers for
faculty recruitment postings from the IITs and IIMs. Then I moved
[commoner-analyse](https://github.com/CommonerLLP/commoner-analyse) and
[public-finance](https://github.com/CommonerLLP/public-finance) onto it so they'd stop maintaining
their own scrapers. It's on [PyPI](https://pypi.org/project/commoner-probe/).

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
