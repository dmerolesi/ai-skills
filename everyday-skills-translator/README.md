# Everyday Skills Translator

A Claude skill that helps people see the professional skills hidden in everyday stories.

## The problem

People undersell themselves. Someone who reorganized a shared space, sorted out a family
schedule, or fixed a recurring problem at home often doesn't recognize that as skill, especially
when changing careers or dealing with impostor syndrome. General-purpose AI tends to make the
opposite mistake: it inflates small tasks into big job titles.

## What it does

1. **Gathers the story** with no more than 3 questions at a time, so it never overwhelms.
2. **Lists 5 to 8 skills** as resume-ready bullets, using standard job-posting language.
   It can target a specific role or stay general.
3. **Shows the evidence and the reasoning** only when the person asks for them.
4. **Runs an inflation check** at all times. If a skill sounds bigger than the story supports,
   it says so, offers a calibrated version, and asks questions that could justify the larger claim.
5. **Handles pushback** by pointing to the concrete action and its workplace equivalent,
   instead of repeating praise.
6. **Turns stories into documents** on request: a case study, a pitch, a LinkedIn post, a cover
   letter paragraph, or a STAR interview answer.

## Design choices

- **Guard against both underclaiming and overclaiming.** The goal is honest, not impressive.
- **Never invent details.** Anything inferred is labeled "(inferred)".
- **The user controls the depth.** Short answers by default, with a menu for going further.

## Example

A story about reorganizing a laundry room for two people of different heights, two cats, and
guests, in a rental where nothing could be drilled into the walls, becomes:

- Designed a shared space around the needs of multiple user groups with different physical needs
- Diagnosed root causes of recurring workflow disruptions and eliminated them
- Implemented a visual inventory system that reduced duplicate purchasing

It would *not* produce "Led facilities management operations." That's a scale mismatch,
and the inflation check would flag it.

## Files

- [`SKILL.md`](SKILL.md): the skill itself

Built with Claude using my guidance.
