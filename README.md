# Consulting Site Best Practices

Value-first approach for consulting sites. Jump straight into usable output. Assume the right customer is already in the room. Demonstrate competence through the work itself. Optional context for those who want it. Continuous handoff so the next step continues what just started.

## Core Principles

- **No warm-up required.** Treat the visitor as a peer who is already a fit. Do not wine-and-dine or explain the method before delivering value.
- **The first interaction is the start of the work.** Collect information by producing something useful, not by running a separate intake form.
- **Competence is shown, not claimed.** The quality and speed of the artifact prove capability.
- **Explanation is opt-in.** Default path has no preamble. A toggle surfaces the why and how only for those who ask.
- **Progress is continuous.** The artifact and context carry forward into the next conversation or call so there is no cold start.
- **Engagement signals fit.** Refining, saving, or continuing the artifact is the qualification. No extra forms.
- **Every CTA is a tool.** Address each call to action with a direct, playable tool that delivers value and collects dogfooding data at the same time.
- **Time-sensitive availability is part of the continuation.** Surface upcoming sessions and remaining spots as concrete next steps, not as pressure.
- **AI agent readiness is the minimum.** If you sell AI services, the site itself must be usable by AI agents. People interested in AI already use it (often without realizing) to look people up, add events to calendars, research, or book. Make the site crawlable and toolable.

## Short-Term Goals (Site Development)

Quick, high-impact changes that establish the value-first path with minimal engineering.

- Replace the default homepage text with a single clear prompt: “Describe what’s in your head that isn’t on the screen yet.” + generate button.
- On submit, immediately return a static or lightly templated artifact (alignment snapshot + 2–3 micro-features + one-day shipping seed) based on the input.
- Add a simple “Show the reasoning” toggle that reveals the existing philosophy, services, about, and diagram content.
- Change the primary CTA to “Continue this” and pre-fill the calendar invite or email with the generated artifact text.
- Add a static or manually updated line under the CTA: “Next available sessions: [date] — X spots left this week.”
- Ensure basic crawlability: valid robots.txt, sitemap.xml, and clean text content so agents can read the page.
- Add minimal structured data (Person or Service schema) for name, offer, and booking method.

## Medium-Term Goals (Site Development)

Deeper tooling that makes the experience live, persistent, and fully agent-receptive.

- Make the artifact generation dynamic (LLM-backed or rule-based refinement that updates live on user edits).
- Add interactive refinement controls (“Narrow the audience”, “Smallest proof”, “Remove this assumption”) that rewrite the artifact in place and log the changes.
- Persist the session (unique link) so the artifact, refinements, and context can be reopened or shared.
- Live availability: real-time or daily-updated spots remaining and next session windows, with a claim-spot or filtered calendar action that attaches the full context.
- Service-mode chips that annotate the artifact and pre-select the handoff type.
- Full AI agent readiness: Markdown content negotiation, API catalog or MCP-style discovery for booking/artifact tools, machine-readable calendar endpoints, and verification against agent-readiness scanners.
- Background structured capture of intent, constraints, refinement history, and preferred session so the handoff is high-context for both human and agent use.

## Default Path (No Preamble)

1. **Direct entry**
   Single clear prompt, no supporting essay:
   
   > Describe what’s in your head that isn’t on the screen yet.
   
   Practical supporting line only: “We’ll generate the first ship and a short plan you can use today.”

2. **Immediate artifact**
   Within seconds return a usable result:
   - Alignment snapshot (gap between mental model and current reality)
   - 2–3 concrete micro-features that could be shipped in the next 1–2 days
   - One-day shipping seed written as next actions

   This is the demonstration. If the output is sharp and actionable, competence is visible without being described.

3. **Optional refinement (still inside the value)**
   One or two quick adjustments appear next to the result:
   - “For users who…”
   - “Smallest piece that proves it”
   - “Adjust this assumption”

   Each change updates the artifact live. No process lecture.

4. **Calls to action that keep moving**
   After the artifact appears:
   - Primary: **Continue this.** (calendar opens with the artifact and notes already attached)
   - Supporting line under the button: “Next available sessions: [date] — 3 spots left this week” (or similar live count)
   - Secondary: Save link / Share / Copy the shipping seed

   After any refinement the primary CTA tightens:
   - **Pick up exactly where this left off.**
   - Same spots-left note remains visible and updates with the booking context.

5. **Handoff with zero reset**
   Booking confirmation and calendar invite carry the generated snapshot, micro-features, and refinement history. The call starts as the next increment, not an introduction. Limited spots make the continuation concrete rather than open-ended.

## AI Agent Readiness (Minimum Requirements)

If the site sells AI consulting or services, it must itself be receptive to AI agents. Most people interested in AI already use it (calendar adds, lookups, research, booking) often without explicitly thinking of it as “using AI.”

Minimum features:
- Clear, crawlable structure and robots.txt / sitemap so agents can discover and index the site.
- Structured data / machine-readable content so agents can extract key info (who you are, what you offer, how to book, availability).
- Calendar or booking endpoints that agents can interact with (add to cal, check spots, book with context).
- Toolable CTAs and interactions (not pure JavaScript walls) so an agent can generate an artifact, refine, or continue on behalf of a user.
- Content accessible in agent-friendly formats where practical (Markdown negotiation, clear text).

Reference check: agent-readiness scanners such as isitagentready.com

The goal is that an AI agent can crawl the site, understand the offer, and help a user take the next step (lookup, calendar add, booking with context) the same way a human can.

## Optional “Why and How” (Off by Default)

A quiet toggle or secondary link: **Show the reasoning.**

When turned on, short inline notes appear beside the artifact:
- Why this micro-feature was chosen
- How the alignment snapshot was derived
- The small-change logic behind the shipping seed

These notes can be collapsed again. They do not interrupt the default path or appear for anyone who hasn’t asked.

## Assumptions

- The visitor who reaches this point is the right customer. No need to sell the value of rapid iteration or prove the approach up front.
- Default experience treats them as a peer already in the room: here is the first ship, refine it if you want, continue when ready.
- Explanation is available on request rather than required.
- Engagement with the artifact (refine, save, book) is the only signal needed. No additional qualification steps.
- Time-sensitive session availability is factual information that helps the right customer act, not a sales tactic.
- AI agents will interact with the site on behalf of users. The site must support that.

## Implementation Notes

- Keep the page short. The work appears immediately.
- The artifact should be shareable and portable (link, one-pager, or downloadable snapshot).
- Structure the background data (intent, constraints, suggested first ship, refinement history) so the handoff is high-context.
- Frame every CTA as continuation of work already done, not as a new sales conversation.
- The site itself dogfoods the principle: it ships a useful response to the visitor’s input before any extended engagement.
- Address each CTA as quickly as possible with a direct tool that lets the visitor play with the value while collecting the data needed for dogfooding.
- Surface time-sensitive upcoming sessions and remaining spots directly under or inside the primary Continue this tool (e.g., live count, next available window, claim-spot button that pre-loads the artifact). Keep the language factual and continuation-oriented.
- Ensure the site meets basic AI agent readiness so that agents can crawl it, extract structured info, and interact with booking or continuation tools. Check against standards such as those measured at isitagentready.com.

## Result

Right customers get straight to usable output and a continuous handoff. Anyone who wants the why and how can turn it on without changing the core experience for everyone else. The first interaction starts the real work and demonstrates competence at the same time. Limited spots and upcoming sessions make the next step concrete without adding friction or preamble. The site is usable by both humans and the AI agents they already rely on.
