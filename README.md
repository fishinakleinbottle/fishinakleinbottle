## Hi, I'm Sreeram

I lead the engineering team and build technology at [Noora Health](https://www.noorahealth.org), where we train family
caregivers across multiple countries in the Global South including India, Indonesia, Bangladesh and Nepal. We are building [digital tools](https://noorahealth.org/tech-that-cares/) for patients, caregivers and healthcare workers that provide timely health information over WhatsApp and IVR. In practice that means a lot of WhatsApp orchestration infrastructure at scale and a lot of content tooling.

I'm also co-building [CommonerLLP](https://commonerllp.org), where we make tools for reading
the Indian state's own paperwork: parliamentary questions, committee reports, budget documents,
public university hiring and so on. The work turns scattered records into public knowledge you can find and
cite, like [theright2read.org](https://theright2read.org) and
[whoseuniversity.org](https://whoseuniversity.org).

Some of my work sits under
[@noorahealthtech](https://github.com/noorahealthtech), my Noora Health account, rather than this
one.

## What I've contributed to

<details>
<summary><strong><a href="https://github.com/Egonex-AI/Understand-Anything">Understand-Anything</a></strong> <a href="https://github.com/Egonex-AI/Understand-Anything/stargazers"><img src="https://img.shields.io/github/stars/Egonex-AI/Understand-Anything?style=social" alt="stars"></a> — turns a codebase into a knowledge graph you can explore and ask questions about</summary>

I swapped its hardcoded TypeScript assumptions for a language and framework registry — 12 languages, 10 frameworks — rebuilt the dashboard navigation around architectural layers, and fixed a bug where parallel analyzer runs produced mismatched node IDs and quietly dropped edges.

</details>

<details>
<summary><strong><a href="https://github.com/andrewyng/context-hub">context-hub</a></strong> <a href="https://github.com/andrewyng/context-hub/stargazers"><img src="https://img.shields.io/github/stars/andrewyng/context-hub?style=social" alt="stars"></a> — a library of documentation written for LLMs rather than for people</summary>

I wrote the Ruby and Rails coverage: ActiveRecord, ActionController, ActiveJob, Devise, Sidekiq, RSpec, FactoryBot, Faraday, and HTTParty.

</details>

<details>
<summary><strong><a href="https://github.com/nyaruka/courier">courier</a></strong> <a href="https://github.com/nyaruka/courier/stargazers"><img src="https://img.shields.io/github/stars/nyaruka/courier?style=social" alt="stars"></a> — the messaging gateway behind RapidPro and TextIt, and what our WhatsApp traffic runs through at Noora Health</summary>

Via [Turn](https://www.turn.io), behind [RapidPro](https://rapidpro.io) and [TextIt](https://textit.com). I fixed the Turn handler dropping header, button, and media components from outgoing templates, and made its 429s retry as throttled rather than fail. Shipped in v26.3.x, authored from [@noorahealthtech](https://github.com/noorahealthtech).

</details>

<details>
<summary><strong><a href="https://github.com/pranaykotas/parliamentwatch">parliamentwatch</a></strong> <a href="https://github.com/pranaykotas/parliamentwatch/stargazers"><img src="https://img.shields.io/github/stars/pranaykotas/parliamentwatch?style=social" alt="stars"></a> — tracks Indian Parliamentary Committee reports from sansad.in</summary>

I added the rosters that were previously buried in report PDFs: 490 members across all 16 standing committees, matched against the Lok Sabha and Rajya Sabha directories and linked to their sansad.in biographies.

</details>

## What I've built

<details>
<summary><strong><a href="https://github.com/CommonerLLP/commoner-probe">commoner-probe</a></strong> <a href="https://pypi.org/project/commoner-probe/"><img src="https://img.shields.io/pypi/v/commoner-probe" alt="PyPI"></a> — handles acquisition for everything we build at CommonerLLP</summary>

Public disclosures sit on undocumented portals with no bulk export and PDFs you can't read programmatically. This deals with that part so the analysis code doesn't have to. On [PyPI](https://pypi.org/project/commoner-probe/).

</details>

<details>
<summary><strong><a href="https://github.com/noorahealthtech/dots-mcp">dots-mcp</a></strong> — puts <a href="https://getdots.in/">DOTS</a>, the knowledge platform we use at Noora Health, behind a chat interface using <a href="https://modelcontextprotocol.io">MCP</a></summary>

The model gets a set of retrieval tools and decides what to search for itself, so the whole knowledge base never has to fit in the context window. It runs in mock mode without credentials, which means you can wire it into Claude and watch the tool calls work before you have a token. Built under [@noorahealthtech](https://github.com/noorahealthtech).

</details>

<details>
<summary><strong><a href="https://github.com/fishinakleinbottle/whatsapp-link-parser">whatsapp-link-parser</a></strong> <a href="https://pypi.org/project/whatsapp-link-parser/"><img src="https://img.shields.io/pypi/v/whatsapp-link-parser" alt="PyPI"></a> — extracts, classifies, and enriches links from WhatsApp chat exports</summary>

Works as a CLI or a Python library, on [PyPI](https://pypi.org/project/whatsapp-link-parser/). It parses several WhatsApp export formats, tags links by type, and pulls page titles and descriptions so a chat's bookmarks are actually searchable.

</details>

## Also working on

<details>
<summary>Private repos — a theatre rehearsal tool, and a Spanish learning platform</summary>

A fair amount of what I spend time on is in private repos

- A rehearsal tool for theatre companies. Script parsing across several formats, annotation, and practice sessions with text-to-speech.
- A [Spanish learning platform](https://plaza.aventurahispana.com/)

</details>
