# Design Notes - Heylo AI landing page

For whoever redesigns this page next. The design is intentionally simple right now and is expected to be improved. The structure and copy rules below are not.

## Structure

- The whole site is one file: `index.html` at the repo root.
- All CSS is inline in a single `<style>` block in the head. No external stylesheets, scripts, fonts, images, or build step. Keep it that way unless there is a strong reason not to: the page must deploy as a plain static site from the repo root.
- Mobile-friendly layout is required. Most visitors are owners on phones.

## Sections, in order

1. Hero: headline "Never miss a customer call again." plus the offer in one breath and the primary call to action.
2. Problem: "The phone rings when you are busiest. That is the problem."
3. How it works (3 steps: intake, build and approval test call, go live).
4. What is included.
5. Pricing: "Simple, honest pricing."
6. Hear it yourself (demo number section).
7. Honest limits, up front (what the AI receptionist does not do).
8. FAQ: "Questions owners ask us."
9. Lead form: "Tell us about your business."

Keep this order and these sections. A redesign may restyle, re-illustrate, and tighten wording, but it may not drop the honest-limits section or the FAQ; they are part of the offer's trust pitch.

Note: a "For individuals" section (personal assistant plan, same Option A pricing) sits between "What is included" and "Pricing." Its text-message price line is pending James's approval; until he approves a number, the page publishes it only as "billed per message" with no price.

## Placeholders that must survive any redesign

- The lead form must keep `action="FORMSPREE_ENDPOINT_PLACEHOLDER"` until a real Formspree endpoint is provided. Do not invent an endpoint, do not point the form at a mailto, and do not remove the form.
- The demo section must keep the literal text `DEMO_NUMBER_PLACEHOLDER` where the demo phone number goes, until a real demo number is provided.
- Form field names are wired to the intake process. Keep the existing `name` attributes on every field (name, business_name, business_type, phone, email, phone_setup, busiest_times, caller_needs, never_say_do, notes).

## Pricing that must not change (Option A)

- Setup: $49 one time.
- Platform fee: $39 per month.
- Talk time: $0.20 per minute, incoming and outgoing, billed per second (never described as rounded up to the next minute).
- No long-term contract, cancel anytime.

Do not add discounts, tiers, strikethrough anchors, or limited-time language. The plain, flat pricing is the pitch.

## Copy rules

- No em dashes anywhere in copy. Use periods, commas, or hyphens.
- No invented testimonials, customer names, logos, review counts, star ratings, call-volume stats, or results claims. There are no public customers yet; the page's proof line is that the owner runs this exact setup on his own business lines, and that stays the only proof claim until real, permissioned testimonials exist.
- No pricing claims beyond the Option A numbers above (for example, do not claim "cheaper than" a named competitor).
- The audience is small businesses, contractors, freelancers, and solo operators. Copy stays plain, warm, and direct, in the owner's voice.
- The service is an AI receptionist and the page says so honestly, including that callers are told it is an AI when they ask. Do not reword the page to imply a human answering service.
