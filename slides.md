---
marp: true
theme: gridsmith
paginate: true
size: 16:9
transition: fade
footer: '![w:28 h:28 GridSmith icon](assets/icon.png) GridSmith · Building a Physical Product in the Age of AI'
---

<!-- _class: title -->
<!-- _paginate: false -->
<!-- _footer: "" -->

![w:112](assets/icon.png)

# GridSmith

## Building a physical product in the age of AI

**A conversation about ideas, iterations, and making real things**

<!--
Open with the finished product in your hands.
"GridSmith is a modular, 3D-printed terrain system for tabletop games."
Frame this as the story of one frustration turning into CAD, manufacturing,
software, and a website. (~1 min)
-->

---

<!-- _class: deck-process -->

# This deck was built with...

<div class="human-ai">
<div>
<span class="role">Human</span>
<strong>Effort + intent</strong>
<p>The story, the judgment, the taste, and the decision to make it.</p>
</div>
<div>
<span class="role">AI</span>
<strong>System + syntax</strong>
<p>Structure, iteration, Markdown, CSS, and the mechanics that made it real.</p>
</div>
</div>

<p class="deck-tools"><strong>ChatGPT</strong> for collaboration · <strong>Marp</strong> for slides · <strong>VS Code</strong> for the live editing loop</p>

<!--
Briefly reveal how the presentation itself was made:
- You supplied the story, goals, feedback, and every meaningful decision.
- ChatGPT helped develop the structure, wording, and implementation.
- Marp turned Markdown and CSS into a presentation.
- VS Code provided the editing and immediate preview loop.

This is a small, recursive example of the talk's central idea. The AI did not
decide that this presentation should exist or what your story meant. It lowered
the friction between your intent and a working artifact. (~1 min)
-->
---

<!-- _class: centered-image-slide -->

<figure><img src="assets/shrek.gif"></figure>

<!--

This talk has a number of layers of nerd.

* D&D
* 3D printing
* Product engineering
* Software engineering
* AI

-->

---

# First, I want to know more about you!

---

# Who here has played D&D or other TTRPGs?

---

# Who here has or has access to a 3D printer?

## Do I need to explain how a 3D printer works?

---

# Who here has mixed the two?

---

<!-- _class: about-builder -->

# I have always been a builder

<p class="about-intro">Most of you know me as the CEO of WWC and general software nerd. However...</p>

<div class="builder-collage">
<figure class="builder-wide"><img src="assets/builder-house.jpg"></figure>
<figure class="builder-red-truck"><img src="assets/builder-red-truck.jpg"></figure>
<figure><img src="assets/builder-50-chevy.jpg"></figure>
<figure><img src="assets/builder-garden.jpg"></figure>
<figure><img src="assets/builder-greenhouse.jpg"></figure>
<figure><img src="assets/builder-wall.jpg"></figure>
<figure class="builder-green-bean"><img src="assets/builder-green-bean-night.png"></figure>
</div>

<!--
This audience already knows your professional identity, so keep that part brief.

Share a couple of quick, specific examples from outside software:
- Working on trucks and learning by taking things apart
- Remodeling houses and solving practical problems as they appeared
- Building computers because understanding the parts was part of the fun
- Growing gardens and improving the setup from one season to the next
- Green Bean, the latest truck project

The common thread is the urge to make, test, adjust, and try again. GridSmith
did not come from nowhere. It gave that lifelong habit a new material and a new
set of tools. (~1.5 min)
-->

---

<!-- _class: dnd-background -->

# D&D gave me another place to build

<div class="dnd-story">
<div class="dnd-copy">
<p><strong>Since 2017</strong><span>I have been playing Dungeons & Dragons.</span></p>
<p><strong>At the table</strong><span>I love homebrewing content and shaping the world around the players.</span></p>
<p><strong>Seven years</strong><span>That is how long my last campaign ran.</span></p>
<p><strong>Beyond the table</strong><span>I built GMBinder.com, which serves tens of thousands of people each month.</span></p>
</div>
<figure class="dnd-photo"><img src="assets/dnd-table.jpg"></figure>
</div>

<!--
This is the other half of the GridSmith origin story.

I started playing D&D in 2017 and quickly found the part of the hobby that fit
me best: making things for the game. I homebrew content, build worlds, and enjoy
giving players something that feels tailored to their story.

My last campaign ran for seven years, so I had a lot of time at the table to
notice what helped the game flow and what got in the way.

That instinct to build also led to GMBinder.com. It gives people a way to create
and share polished homebrew documents, and it now serves tens of thousands of
people every month.

GridSmith grew from both sides of my background: I like building, and I care
deeply about the experience around a D&D table. (~2 min)
-->

---

<!-- _class: sample-slide -->

# Years ago... I printed hundreds of tiles

<p class="sample-lead">I knew these systems as a user long before I tried to become a designer.</p>

<div class="old-tiles-gallery">
<figure class="old-tiles-wide"><img src="assets/old-tiles-tavern.jpg"></figure>
<figure><img src="assets/old-tiles-dungeon.jpg"></figure>
<figure><img src="assets/old-tiles-room.jpg"></figure>
</div>

<!--
Start passing the older tile-system samples around now. Let them continue
moving through the room during the next slide.

Explain that you genuinely liked and used these systems. This is not a teardown
of somebody else's work; it is the perspective of a heavy user who learned
where the tradeoffs lived by printing hundreds of pieces.

Ask the audience to notice three physical details:
- How thick and heavy the base is
- How a wall occupies part of the floor tile
- How the tile shapes constrain what can be assembled

The samples make the problem tangible before you introduce your answer. (~2 min)
-->

---

<!-- _class: gridfinity-inspiration -->

# One day I was printing Gridfinity grids for my silverware drawer...

<div class="gridfinity-sequence">
<figure><span>01</span><img src="assets/gridfinity-evolution-01.jpg"></figure>
<figure><span>02</span><img src="assets/gridfinity-evolution-02.jpg"></figure>
<figure><span>03</span><img src="assets/gridfinity-evolution-03.jpg"></figure>
<figure><span>04</span><img src="assets/gridfinity-evolution-04.jpg"></figure>
<figure><span>05</span><img src="assets/gridfinity-evolution-05.jpg"></figure>
<figure><span>06</span><img src="assets/gridfinity-evolution-06.jpg"></figure>
</div>

<!--
Gridfinity provided the conceptual spark. Its organizing idea is simple: a
standard grid creates structure, while interchangeable pieces drop into it.

You wondered whether the same separation could work for terrain. Instead of
asking every floor tile to carry its own structure and connections, could a
thin grid underneath do that job?

Walk through these images in order. You were not designing finished terrain
yet. You were testing the architecture by building frames around tiles you
already owned and had printed hundreds of times.

Each version answered a physical question:
- Does the grid hold the tile?
- How much frame is actually necessary?
- Where does the fit become too loose or too tight?
- Can old content become modular without reprinting everything?

The progression matters more than any individual frame. This was the moment
the idea shifted from "make a better tile" to "build a system underneath the
tiles." (~2 min)
-->

---

<!-- _class: gridfinity-inspiration -->

# And I had some terrain tiles laying on my desk

## If it fits, it sits.

<div class="gridfinity-sequence">
<figure><span>01</span><img src="assets/old_1.jpg"></figure>
<figure><span>02</span><img src="assets/old_2.jpg"></figure>
<figure><span>03</span><img src="assets/old_3.jpg"></figure>
<figure><span>04</span><img src="assets/old_4.jpg"></figure>
<figure><span>05</span><img src="assets/old_5.jpg"></figure>
</div>


---

<!-- _class: centered-image-slide -->

<figure><img src="assets/but_wait.jpeg"></figure>

---

<!-- _class: centered-image-slide -->

<figure><img src="assets/3_months.jpg"></figure>

---

# I started to question what I had created.

## I mean... there were issues with the 100s of tiles I had printed

## And I wanted new tiles.

---


# Old tiles didn't seem ideal

<div class="frictions">
<div><strong>Too much plastic and waiting</strong><span>Excessive thickness consumed filament and added print time across every tile.</span></div>
<div><strong>Too little floor</strong><span>Walls consumed half a tile, shrinking the playable space you just printed.</span></div>
<div><strong>Too few layouts</strong><span>The system struggled with narrow hallways and other useful configurations.</span></div>
<div><strong>Too complicated</strong><span>Connecting tiles required magnets, glue, or brittle clips.</span></div>
</div>

<p class="friction-summary">Material and time. Playable space. Flexibility. Assembly.</p>

<!--
Use the samples as evidence while you walk through the four constraints.

Excessive thickness and print time:
- Material was being spent where it did not improve the play experience.
- A small amount per tile becomes substantial across hundreds of tiles.
- Thickness means layers, and layers mean time.
- Building a usable room or dungeon required committing the printer for a long
  time before play could begin.

Floor efficiency:
- When the wall shares the floor tile, it consumes a meaningful part of the
  playable square.
- You pay to print floor area that cannot really be used.

Layout flexibility:
- Wall and floor geometry are coupled.
- Narrow hallways and other common layouts become awkward or impossible.

Assembly complexity:
- Magnets added parts, cost, glue, and installation time.
- Printed clips could be fiddly and brittle.
- Building the terrain should not require another construction project first.

The insight: these were not unrelated annoyances. They came from the structure
and assembly model of the system. (~2.5 min)
-->

---

<!-- _class: statement -->

# What if terrain could use less - and do more?

## Less filament. Less waiting. More usable floor. More ways to build.

<!--
This is the product-design challenge distilled from the samples.

GridSmith would need to change the underlying geometry, not merely make a
prettier version of the same tile. Refer back to this promise when you discuss
thin parts, separate walls, print time, and hallway layouts. (~1 min)
-->

---

# So I asked the dangerous question

<div class="big-quote">"How hard would it be<br>to create my own?"</div>

<p class="muted">A reasonable question with a wildly unreasonable answer.</p>

<!--
You had enough experience to see the problems, but no background as a CAD
designer or manufacturing engineer.

That gap is what made this both a product idea and a perfect AI experiment:
could you use AI to cross into an unfamiliar discipline and make a real,
physical system of your own? (~1 min)
-->

---

<!-- _class: statement dark -->

# I wanted to use AI on something real

## Not another "build me a..."  prompt

# I wanted a physical system

## with code, constraints, failures, and consequences.

<!--
GridSmith was deliberately an experiment in using AI more robustly:
- Could it stay useful across a long-running, multi-disciplinary project?
- Could it help move between product thinking, CAD, manufacturing, writing,
  branding, and web development?
- Could the collaboration survive contact with the physical world?

Position AI as a persistent collaborator, not an answer machine. It accelerated
exploration, but you still chose the direction and owned every result. (~1.5 min)
-->

---

<!-- _class: initial-requirements -->

# First, I gathered requirements

<p class="requirements-lead">If I was going to build my own system, it had to...</p>

<div class="requirements-list">
<div><span>01</span><p><strong>Use less material</strong>Every millimeter needed to earn its place.</p></div>
<div><span>02</span><p><strong>Print faster</strong>A useful room could not take forever to produce.</p></div>
<div><span>03</span><p><strong>Preserve every square</strong>Walls could not consume half the playable floor.</p></div>
<div><span>04</span><p><strong>Support flexible layouts</strong>Hallways, small rooms, and odd shapes had to work.</p></div>
<div><span>05</span><p><strong>Drop into place</strong>No magnets, clips, or fiddly connectors.</p></div>
<div><span>06</span><p><strong>Print reliably</strong>Simple, repeatable parts that worked on an FDM printer.</p></div>
</div>

<!--
This is a reconstructed first pass at the requirements based on the problems
you had already identified. Adjust the wording to match the list you actually
carried into the first design sessions.

The important shift was turning frustration into constraints. You were no
longer asking AI to invent some terrain. You had a definition of better:
- less plastic and less print time
- the whole grid remained playable
- layouts included hallways and smaller spaces
- assembly stayed simple, without separate hardware
- the parts could be printed repeatedly and predictably

Those constraints gave the AI something useful to reason against, and they
gave every physical prototype a pass-or-fail test. (~2 min)
-->

---

<!-- _class: cad-first-step -->

# Then I reverse engineered

<p class="cad-origin">I gave ChatGPT an STL from a tile set I had already printed hundreds of times.</p>

<div class="cad-origin-flow">
<div><span>01</span><strong>Start with the STL</strong><small>A familiar object, but no editable design behind it.</small></div>
<b>→</b>
<div><span>02</span><strong>Ask a few questions</strong><small>ChatGPT helped unpack the geometry and pointed me toward OpenSCAD.</small></div>
<b>→</b>
<div><span>03</span><strong>Render something new</strong><small>Within a couple of prompts, I had my first CAD prototype.</small></div>
</div>

<p class="lost-prototype"><strong>No screenshot survived.</strong> I did not know yet that this was the beginning of the story.</p>

<!--
The first action was not to design GridSmith from scratch. It was to start with
something familiar: an STL from an older tile you had printed hundreds of times.

You asked ChatGPT to help reverse engineer it. Within a couple of prompts, the
conversation pointed you toward OpenSCAD and produced enough code to render a
first CAD prototype.

That surprised you. CAD had always felt like a specialized skill with a steep
entry cost. Suddenly, you had crossed the first barrier without a class, a
tutorial series, or months spent learning a traditional modeling interface.

Be honest about the missing artifact: there is no screenshot because this did
not feel historically important in the moment. It was simply the first thing
that worked. (~2 min)
-->

---

# OpenSCAD became our shared language

<div class="columns">
<div class="placeholder wide">
  <img src="assets/2.png">
</div>
<div class="placeholder wide">
  <img src="assets/3.png">
</div>
</div>

<!-- IMAGES: Replace the two placeholders above with:
![w:520](assets/openscad-script.png)
![w:520](assets/openscad-output.png)
-->

<p class="caption">I supplied intent and judgment. AI supplied speed and syntax. The printer supplied truth.</p>

<!--
First explain OpenSCAD in plain language:
- It creates 3D geometry from text-based code.
- Modules describe reusable parts; parameters control dimensions and behavior.
- Change a number, render again, and the model updates predictably.

Then explain why it became an effective human–machine interface:
- You defined the goal, constraints, taste, and what "good" felt like.
- AI could read and generate the same textual design language.
- You reviewed the logic and chose what was worth printing.
- The print returned evidence neither human nor AI could simulate perfectly:
  fit, strength, finish, friction, and feel.

The compelling point is not simply that AI wrote OpenSCAD. OpenSCAD gave the
human and AI a shared, editable representation of the product. (~2.5 min)
-->

---

# Version one was… a version

<div class="columns">
<div class="placeholder square">
  <img src="assets/1.jpg">
</div>
<div class="side-copy">
<p class="huge">Not impressive.</p>
<p>But it proved the idea could become an object.</p>
</div>
</div>

<!-- IMAGE: Replace the first placeholder above with:
![w:470](assets/prototype-first.jpg)
-->

<!--
Show the genuinely rough beginning. Explain what was wrong: fit, scale, print
time, strength, appearance, or all of the above. (~1 min)
-->

---

# The loop crossed two worlds

<div class="loop">
<div><span>1</span>Describe</div><b>→</b>
<div><span>2</span>Generate</div><b>→</b>
<div><span>3</span>Print</div><b>→</b>
<div><span>4</span>Learn</div>
</div>

<p class="big-center">Then feed reality back into the next conversation.</p>

<!--
Give one concrete connector or tolerance example. AI proposed geometry, you
printed it, reality exposed a constraint, and the loop repeated. (~2 min)
-->

---

# The prompt was never the product

<div class="columns">
<div class="placeholder tall">
  <img src="assets/4.jpg">
</div>
<div class="side-copy">
<p class="huge accent">The print was the test.</p>
<p>Plastic settled every argument about fit, strength, and feel.</p>
</div>
</div>

<!-- IMAGE: Replace the first placeholder above with:
![w:520](assets/ai-conversation.png)
-->

<!--
Contrast vibe coding software with vibe coding a physical product. Generated
code can look right and still print badly. Share a memorable example. (~1.5 min)
-->

---

<!-- _class: photo -->

# Print. Wait. Fail. Repeat.

<div class="photo-collage">
<img src="assets/5.jpg" alt="GridSmith prototype 5">
<img src="assets/6.jpg" alt="GridSmith prototype 6">
<img src="assets/7.jpg" alt="GridSmith prototype 7">
<img src="assets/8.jpg" alt="GridSmith prototype 8">
<img src="assets/9.jpg" alt="GridSmith prototype 9">
<img src="assets/10.jpg" alt="GridSmith prototype 10">
<img src="assets/11.jpg" alt="GridSmith prototype 11">
<img src="assets/12.jpg" alt="GridSmith prototype 12">
</div>

<!--
Tell two short failure stories. Each failure purchased information: name the
assumption it disproved and the change it caused. (~1.5 min)
-->

---

# Millimeters became product decisions

## A spec was forming

<div class="comparison">
<div><span>0.1 mm</span><p>Too tight</p></div>
<div><span>0.2 mm</span><p>Promising</p></div>
<div><span>0.3 mm</span><p>Too loose</p></div>
</div>

<!-- OPTIONAL IMAGE: Replace the comparison above with:
![w:1050](assets/tolerance-test.jpg)
-->

<!--
Replace these numbers with a real example. Discuss tolerances, elephant's foot,
layer lines, material behavior, or calibration. (~1.5 min)
-->

---

# The slicer is where design meets reality

<div class="columns">
<div class="placeholder wide">
  <img src="assets/13.png">
</div>
<div class="placeholder wide">
  <img src="assets/14.png">
</div>
</div>

<!-- IMAGES: Replace the two placeholders above with:
![w:520](assets/orcaslicer.png)
![w:520](assets/creality-print.png)
-->

<!--
Define a slicer in one sentence. Explain how orientation changes strength and
finish, supports cost time, and small changes compound across a batch. (~1.5 min)
-->

---

<!-- _class: photo -->

# One prototype became a tiny factory

<div class="placeholder hero">
  <img src="assets/hero.gif">
</div>

<!-- IMAGE: Replace the placeholder above with:
![w:1120](assets/printer-production.jpg)
-->

<!--
Cover the printer evolution, K2 + CFS, print hours, filament, consistency,
batching, machine babysitting, packaging, and inventory. (~2 min)
-->

---

# Software bugs can be patched

<div class="two-lines">
<p>A bad print wastes <strong>hours.</strong></p>
<p>A bad batch wastes <strong>a weekend.</strong></p>
</div>

<!--
Let the contrast land. Explain how matter encouraged smaller tests, deliberate
validation, repeatability, and respect for production constraints. (~1 min)
-->

---

<!-- _class: statement -->

# At some point, the project needed a name

## Grid + craft + system → **GridSmith**

<!--
Tell the naming story if there is one. This is the pivot from experiment to
product: branding, packaging, instructions, and someone else using it. (~1 min)
-->

---

<!-- _class: photo -->

# Meet GridSmith


<div class="placeholder hero contain">
  <img src="assets/hero.png">
</div>

<!--
Show the destination before the journey. Point out the base grid, tiles,
walls, props, and trays. Drop a tile into the grid if you brought one. (~1 min)
-->

---

# The physical product needed a digital home

<div class="placeholder browser">
  <img src="assets/landing.png">
</div>

<!-- IMAGE: Replace the placeholder above with:
![w:1120](assets/website-home.png)
-->

<!--
The website became a second product, not just checkout. What did it need to
explain that was obvious when holding the pieces? (~1 min)
-->

---

# I wanted tools - not just pages

<div class="feature-pair">
<div>
<div class="feature-frame"><img src="assets/15.png" alt="GridSmith Tile Builder"></div>
<strong>Tile Builder</strong>
<span>Design a tile, preview the geometry, and export the STL - all in the browser.</span>
</div>
<div>
<div class="feature-frame"><img src="assets/16.png" alt="GridSmith Grid Builder"></div>
<strong>Grid Builder</strong>
<span>Plan the playable space before committing hours and filament to a print.</span>
</div>
</div>

<!--
Frame these as capabilities you wanted to exist, not requirements handed to
you by a product manager.

Tile Builder:
- Let someone shape a useful part without learning OpenSCAD.
- Run OpenSCAD through WASM locally in the browser.
- Preview and export the STL without sending CAD work to a server.
- Turn the parametric system you built for yourself into a tool other people
  could use.

Grid Builder:
- Planning should happen before printing.
- Help people reason about rooms, coverage, and the pieces they actually need.
- Reduce wasted filament and abandoned prints by moving experimentation into
  the browser.

The larger idea: the website began reflecting the same GridSmith principle as
the physical product - remove friction between an idea and play. (~2 min)
-->

---

# I wanted buying terrain to feel just as direct

<div class="feature-wide">
<img src="assets/17.png" alt="GridSmith shopping experience">
</div>

<p class="feature-caption"><strong>Discover.</strong> Choose. Own. Download - or order the physical set.</p>

<!--
Explain the shopping experience you wanted:
- One place for physical sets, printable tile packs, and tools.
- A catalog that makes the system understandable rather than exposing a pile
  of disconnected files.
- Stripe Checkout for the transaction.
- Cognito-backed ownership so the site knows which packs a customer owns.
- Private S3 files delivered through presigned download URLs.

This is where the four-system architecture becomes a user experience:
Vercel presents the shop, Cognito knows the customer, Stripe records the
purchase, and AWS grants access to the files.

Keep the focus on the experience you wanted to create; the implementation is
evidence that you could build it. (~1.5 min)
-->

---

# The website is really four systems

<div class="system-map">
<div><strong>Vercel</strong><span>Website + builders</span></div>
<div><strong>AWS</strong><span>Commerce API + tile pack files</span></div>
<div><strong>Stripe</strong><span>Money + catalog</span></div>
<div><strong>Cognito</strong><span>Who you are</span></div>
</div>

<p class="tech-foundation"><strong>In the browser:</strong> React 18 + TypeScript · PrimeReact · OpenSCAD WASM · MDX</p>
<p class="tech-foundation"><strong>Shipping it:</strong> Webpack · GitHub Actions · Node 24</p>

<!--
Start with the mental model; it makes the implementation easier to follow:
- Vercel is the website and the interactive builders.
- AWS is the authenticated commerce API and protected pack files.
- Stripe owns money, prices, Checkout, receipts, and the product catalog.
- Cognito answers who the user is.

Frontend / app:
- React 18 single-page app written in TypeScript and bundled with Webpack.
- PrimeReact, PrimeFlex, and PrimeIcons provide the UI system.
- Marketing pages, shop, and builders all live in the same client app.
- OpenSCAD runs as WASM in the browser. Baseplate and tile builders can preview
  models and export STL files without server-side CAD.
- Build-log posts are MDX compiled into the application bundle with
  @mdx-js/loader and @mdx-js/react.

Hosting:
- Vercel serves the static SPA from `npm run build:all`.
- Environment variables provide Cognito configuration and
  GRIDSMITH_API_BASE_URL.
- The blog build generates a sitemap and can optionally prerender `/blog`
  routes after the main build.

Identity:
- Amazon Cognito Hosted UI supports authentication, including Google.
- The browser holds the ID token.
- The Cognito pool and client must match the configuration verified by the API
  Lambdas.

Commerce / API:
- API Gateway and Lambda are defined with SAM under `infra/api`.
- Separate dev, staging, and production stages.
- Stripe credentials come from Secrets Manager through STRIPE_SECRET_ARN.
- Core endpoints cover catalog, Checkout sessions, owned-pack capabilities,
  and presigned tile-pack download URLs.
- Each stage has a private S3 bucket for purchased files; downloads use
  presigned GET URLs.

Delivery and testing:
- GitHub Actions can deploy through OIDC to IAM; local
  `npm run deploy:api:*` commands are also available.
- CI runs test/build workflows separately from API deployment.
- The toolchain is Node 24 with Jest and Puppeteer end-to-end coverage,
  although e2e is often skipped in CI for now.

This is a tour of responsibilities, not a request for the audience to memorize
the stack. The surprising detail worth lingering on is OpenSCAD WASM: the
browser is performing real CAD work locally. (~2.5–3 min)
-->

---

<!-- _class: statement dark -->

# Vibe coding the website

## Let’s open Cursor. - No, let's not.

<!--
Leave the deck and open the GridSmith project in Cursor.

Show one end-to-end website story:
- The intent or problem you described
- How Cursor explored the existing codebase
- The proposed or generated change
- The browser result
- What still required your judgment

Keep the live portion bounded. The goal is to show the collaboration loop, not
to complete a risky feature in front of the audience. (~3–4 min)
-->

---

# The website had its own sharp edges

<div class="edges">
<p>Product photography</p><p>Image performance</p>
<p>Explaining the system</p><p>SEO & discovery</p>
<p>Content automation</p>
</div>

<!--
Choose 2–3 strong stories: images without slow pages; explaining a tactile
system; reusable content; deployment; or reviewing plausible AI output. (~1.5 min)
-->

---

# What surprised me most

<div class="lessons">
<p><strong>AI amplified engineering.</strong><br>It did not remove the need for it.</p>
<p><strong>Iteration beat expertise.</strong><br>Momentum made the unfamiliar learnable.</p>
<p><strong>Physical feedback changed everything.</strong><br>Reality was always in the loop.</p>
</div>

<!--
Keep this reflective and personal. Rewrite anything that is not authentic to
your experience. (~2 min)
-->

---

<!-- _class: statement dark -->

# One person became a small product team

## CAD modeler · Manufacturing Engineer · Web Developer · Writer · Photographer · Marketer

<!--
The point isn't mastery of every discipline. AI lowered the activation energy
enough to participate in all of them and keep moving. (~1 min)
-->

---

# The AI story pauses here. The iteration didn’t.

<div class="product-evolution-grid">
<figure><img src="assets/2_tone_tile.jpg"></figure>
<figure><img src="assets/printer_2.jpg"></figure>
<figure><img src="assets/final.jpg"></figure>
<figure><img src="assets/store.jpg"></figure>
<figure><img src="assets/case_5.jpg"></figure>
</div>

<!--
Move through this quickly. The point is not another deep product section.
The physical work kept evolving: two-color pieces, more capable printers,
repeatable batches, and eventually putting the product in front of people.
(~30–45 sec)
-->

---

# Even the case became a prototype

<div class="case-evolution-grid">
<figure><img src="assets/case_1.jpg"><span>01</span></figure>
<figure><img src="assets/case_2.jpg"><span>02</span></figure>
<figure><img src="assets/case_3.jpg"><span>03</span></figure>
<figure><img src="assets/case_4.jpg"><span>04</span></figure>
<figure><img src="assets/case_6.jpg"><span>05</span></figure>
</div>

<!--
No AI lesson here, just the same habit carrying forward: build it, handle it,
notice what is wrong, and make the next version. Let the sequence tell the
story rather than explaining every change. (~30–45 sec)
-->

---

<!-- _class: closing -->
<!-- _paginate: false -->
<!-- _footer: "" -->

# In the end... AI lowered the barrier.

## Iteration built the product.

### And now there’s a real thing on the table.

<!--
Return to the physical object and click a tile into place.
"The exciting part isn't that AI built GridSmith for me. It's that AI lowered
the barrier enough that I finally built the thing I'd been thinking about."
Invite questions. (~1 min)
-->

---

<!-- _class: centered-image-slide -->

<figure><img src="assets/5_months.jpg"></figure>

---

# Gridsmith is currently living the fate of many of my hobbies...

## I do have a desire to pick it back up, but there are only so many days in the week.

---

# What’s next on the workbench?

<div class="roadmap">
<p>More environments</p><p>Print Planner</p>
<p>Better production workflows</p><p>More automation</p>
</div>


<!-- IMAGE: Replace the placeholder above with:
![w:1120](assets/future-teaser.jpg)
-->

<!--
Only mention work you genuinely expect to pursue. Explain Print Planner in one
sentence and save a demo for Q&A. (~1 min)
-->

---

<!-- _class: feedback -->

# Help me sharpen the next version of this talk

<div class="feedback-questions">
<div>
<span>01</span>
<strong>What is missing - or what could I elaborate on?</strong>
</div>
<div>
<span>02</span>
<strong>What could be removed?</strong>
</div>
</div>

<!--
Open the floor for candid feedback rather than general Q&A.

First question:
"Do you think this is strong enough - and useful enough - for the AI User Group?"

Second question:
"What felt missing, rushed, or worth going deeper on?"

Listen especially for:
- Places where the story assumes too much technical knowledge
- Moments where a real example would be stronger than a summary
- Questions about the human/AI working relationship
- Which live or physical demonstrations created the most value

Capture the feedback after the session so this lunch & learn becomes the first
iteration of the user-group talk. (~3–5 min)
-->

---

<!-- _class: code-camp-promo -->

<div class="code-camp-layout">
<figure class="code-camp-spotlight"><img src="assets/iowa-code-camp-levi-rosol.png"></figure>
<div class="code-camp-invite">
<p class="code-camp-kicker">Iowa Code Camp · November 7, 2026</p>
<h1>Let’s continue the conversation</h1>
<p>I’ll be giving this talk again in Ankeny.</p>
<img class="code-camp-qr" src="assets/iowa-code-camp-qr.png">
<strong>iowacodecamp.com</strong>
</div>
</div>

<!--
If someone in the room knows a developer, maker, or AI-curious person who would
enjoy this story, invite them to join you at Iowa Code Camp in November.

The QR code opens the Iowa Code Camp website. (~30 sec)
-->

---

<!-- _class: thank-you -->
<!-- _paginate: false -->
<!-- _footer: "" -->

<div class="thank-you-copy">
<img src="assets/icon.png" alt="GridSmith shield">
<h1>Thank you</h1>
<h2>gridsmith.io</h2>
</div>

<div class="thank-you-repo">
<img src="assets/github-repo-qr.png" alt="QR code for the GridSmith presentation repository">
<strong>Get the deck</strong>
<span>github.com/LeviRosol/<br>gridsmith-dev-session</span>
</div>

<!--
End here after the feedback discussion.

Thank everyone for their time, for handling the samples, and for helping you
improve the next version of the talk.
-->

<script>
(() => {
  if (document.querySelector('.image-lightbox')) return;

  const lightboxStyles = document.createElement('style');
  lightboxStyles.textContent = `
    .image-lightbox {
      position: fixed;
      z-index: 99999;
      inset: 0;
      display: none;
      align-items: center;
      justify-content: center;
      box-sizing: border-box;
      padding: 44px;
      background: rgba(0,0,0,.92);
      cursor: zoom-out;
    }
    .image-lightbox.open { display: flex; }
    .image-lightbox img {
      width: auto;
      height: auto;
      max-width: 94vw;
      max-height: 90vh;
      object-fit: contain;
      cursor: default;
      filter: drop-shadow(0 18px 44px rgba(0,0,0,.75));
    }
    .image-lightbox-close {
      position: fixed;
      z-index: 100000;
      top: 18px;
      right: 26px;
      padding: 0;
      color: #fff;
      background: transparent;
      border: 0;
      font: 300 48px/1 Arial, sans-serif;
      cursor: pointer;
    }
  `;
  document.head.appendChild(lightboxStyles);

  const lightbox = document.createElement('div');
  lightbox.className = 'image-lightbox';
  lightbox.setAttribute('role', 'dialog');
  lightbox.setAttribute('aria-modal', 'true');
  lightbox.setAttribute('aria-label', 'Expanded slide image');
  lightbox.innerHTML = '<button class="image-lightbox-close" type="button" aria-label="Close image">&times;</button><img alt="">';
  document.body.appendChild(lightbox);

  const expandedImage = lightbox.querySelector('img');
  const close = () => {
    lightbox.classList.remove('open');
    expandedImage.removeAttribute('src');
  };

  document.addEventListener('click', event => {
    const image = event.target.closest('section img');
    if (!image || image.closest('footer') || image.closest('.image-lightbox')) return;

    event.preventDefault();
    expandedImage.src = image.currentSrc || image.src;
    expandedImage.alt = image.alt || 'Expanded slide image';
    lightbox.classList.add('open');
  });

  lightbox.addEventListener('click', event => {
    if (event.target === lightbox || event.target.closest('.image-lightbox-close')) close();
  });

  window.addEventListener('keydown', event => {
    if (event.key !== 'Escape' || !lightbox.classList.contains('open')) return;

    event.preventDefault();
    event.stopPropagation();
    event.stopImmediatePropagation();
    close();
  }, true);
})();
</script>
