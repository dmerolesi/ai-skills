# AI Skills

Skills I've designed for AI assistants. A skill is a set of written instructions that teaches an
assistant like Claude how to handle one kind of task well, every time.

I decide what each skill should do and how it should behave, and Claude helps turn that guidance
into clear written instructions.

## Skills

| Skill | What it does |
|-------|--------------|
| [Everyday Skills Translator](everyday-skills-translator/) | Turns everyday stories into honest, resume-ready skills, with built-in checks against overclaiming |

## How to use a skill

Each skill lives in its own folder with a `SKILL.md` file. To use one with
[Claude Code](https://claude.com/claude-code), copy the folder into `~/.claude/skills/`.
Claude then uses the skill automatically when a request matches its description.

More about this work at [dana.lovellcrew.us](https://dana.lovellcrew.us).
