# Coastline Heat Pumps Homepage

_Started 2026-04-29 12:21 UTC_

---

## User

I need you to design the homepage for a fictional UK heat pump installer called Coastline Heat Pumps. This is a portfolio/mockup project — the company isn't real, but the design should be production-ready quality. Treat it as a real client brief.
The business in one paragraph
Coastline Heat Pumps is a six-person specialist installer based in Truro, Cornwall, serving Cornwall and South Devon. They install air source heat pumps and solar PV, primarily replacing oil and LPG boilers in rural Cornish properties. Founded in 2018, MCS-certified, BUS-approved (the £7,500 UK government grant for heat pump installations).
The audience this homepage must convince
A specific person: a Cornish or South Devon homeowner aged 45–65, currently using oil or LPG heating in a 3–5 bedroom rural property. Their boiler is 10+ years old, fuel bills hurt, they've heard about the £7,500 government grant. They've Googled "heat pump installer Cornwall" and they're comparing 2–3 local installers. They're cautious — this is a £15,000+ decision. They will dismiss any installer whose website looks amateur, generic, or templated. They respect understatement and specificity. They distrust marketing fluff.
The design philosophy
Quiet competence. The aesthetic should feel closer to a thoughtful boutique architect or specialist solicitor than a tradesman site or tech startup. Generous whitespace, calm typography, restrained colour, real photography. Conservative without being boring. Modern without being trendy. When in doubt, remove rather than add. If the site feels slightly less designed than competitors, you've calibrated correctly.
Reference points for tone (not for visual copying): Stripe's clarity with technical content, Linear's typographic restraint, the calm credibility of a specialist UK consultancy site like Carbon Intelligence. Avoid: typical heat pump installer sites, generic SaaS landing pages, anything that looks templated.

## Assistant

I'll read the design system's UI kit to understand the existing components and visual vocabulary, then build the homepage.

_[tool: list_files]_

_[tool: read_file]_

Now let me look at the existing UI kit components and key preview pieces to understand the visual vocabulary before building.

_[tool: read_file]_

I have enough context. Let me check the logo and a couple more pieces, then build.

_[tool: list_files]_

_[tool: read_file]_

I have what I need. Let me copy the logo and fonts CSS into this project, then build the homepage.

_[tool: copy_files]_

_[tool: snip]_

Now I'll build the full homepage. The brief is detailed and specific — I'll execute it faithfully, with the desktop page first and mobile views for sections 1 & 3 appended at the bottom.

_[tool: write_file]_

_[tool: snip]_

Now the HTML file. I'll write it as canonical HTML (no React needed — this is a wireframe/marketing page that benefits from being editable).

_[tool: write_file]_

## Assistant

Now the HTML page:

_[tool: write_file]_

## Assistant

Now the HTML page itself.

_[tool: write_file]_

_[tool: snip]_

_[tool: done]_

_[tool: fork_verifier_agent]_

Built the Coastline homepage — all eight sections in the brief order, plus mobile renders of the hero and How it works at 375px below the desktop view.

**A few calibration notes for review:**

- **Photo placeholders are annotated**, not generic — each one names the subject, light, and framing (e.g. *"1920s granite cottage exterior, overcast Cornish light, heat pump unit visible on side wall"*).
- **Copper appears exactly three times** above the fold zone (nav, hero primary, "Start step 1") and once in the closing CTA. Tertiary links use Slate Blue, not Copper, to keep the warm note scarce.
- **Hero is centred**, photo is contained at 16:7 with subtle radius — not full-bleed, no overlay text.
- **Section 8** is set against `#2E4756` Slate Blue with the lead in Coastal Mist `#6B8693` exactly per the brief.
- **FAQ accordions** are interactive — click any question to expand.
- **Two fonts only**: Fraunces for H1/H2/install card titles, Inter for everything else.

If anything reads as over-designed, the most likely culprits are the photo-placeholder hatching pattern (could go flat Stone) or the section eyebrows (could drop to plain section spacing). Easy strips if you want them quieter.

## User

all good, but we need a team section as well, and there should be an option for a video, I want to play the video of team members ( I will create it in AI) to make an example of good videos that actually promote a team

## Assistant

_[tool: snip]_

_[tool: read_file]_

I'll add a Team section with a video player as the centerpiece, slotted between Why Us (Section 6) and FAQ (Section 7) — that's the natural emotional beat for "meet the people."

Let me add the CSS for the team section first, then insert the HTML.

_[tool: str_replace_edit]_

_[tool: snip]_

_[tool: str_replace_edit]_

Now I'll renumber FAQ and CTA labels and update the script to handle video play, plus update the FAQ data-screen-label since team is now 07.

_[tool: str_replace_edit]_

_[tool: snip]_

_[tool: done]_

Added a Team section between Why Us and FAQ. Here's what's there:

- **A 16:9 video card** with a Copper play button, an annotated poster ("Replace with team film · 90 seconds — workshop in Truro, on-site fitting at a granite cottage, brief pieces-to-camera, cool overcast light"), and a corner caption *"Meet the team — 1:32"*. Clicking the card swaps the poster out and plays `assets/team-intro.mp4` once you drop your AI-generated video at that path. If the file's missing it stays on the poster — no error.
- **Six team cards** below in a 3-up grid (4:5 portrait placeholders, name, role in Copper, one line of plain-spoken provenance — MCS dates, F-Gas, Truro & Penwith College apprenticeship, etc).
- **Section heading**: *"Six people. All in Cornwall."* with a one-line lede about no subcontractors — keeping the quiet-competence tone.

To use your video: save it to `assets/team-intro.mp4`. If you'd prefer a different filename or want me to wire it up for an external host (Vimeo, Mux, etc.), say the word.

## User

now I need another page with a quote calculation plugin, so you will need to create another page and this plugin.

## Assistant

