# my-claude-skills

A collection of Claude skills built by [@wenyuanwu](https://github.com/wenyuanwu). Each skill is a prompt instruction file that customizes Claude's behavior for a specific use case.

---

## Skills

### 🎯 pm-interview-coach

An expert PM interview coach powered by the **Ben Erez / Lenny's Newsletter product sense framework**. It evaluates your answers and helps you practice for product sense interviews at top tech companies (Google, Meta, Stripe, etc.).

#### What it does

**Evaluates your answers** across 5 dimensions, each scored 1–5:
- **Clear Communication** — Is your structure crisp? Do you state a game plan upfront and signpost between sections?
- **Product Motivation** — Do you articulate *why* the product exists, its strategic position, and the human value it delivers?
- **Segmentation** — Do you define motivation-based user segments (not just demographics) and argue which is most underserved?
- **Problem Identification** — Do you identify a specific problem with frequency × severity logic, tied back to the product mission?
- **Solution Development** — Do you propose a concrete v1 with impact × effort reasoning, risks, and platform leverage?

**Gives you a verdict:** Strong Pass / Pass / Borderline / Fail — with honest, direct feedback tied to specific moments in your answer.

**Offers a model answer example** — After every evaluation, it asks if you'd like a model answer that directly targets your weakest areas. If yes, it generates a full answer with a "What to steal" section highlighting the specific moves you should incorporate.

**Generates model answers from scratch** — Ask it to demo a strong answer for any product and it will walk through the full skeleton.

---

## How to Download & Use

### Step 1: Download the skill

Clone this repo or download the folder directly:

```bash
git clone https://github.com/wenyuanwu/my-claude-skills.git
```

Or download just the skill file:
- Go to [`pm-interview-coach/SKILL.md`](./pm-interview-coach/SKILL.md)
- Click **Raw** → Save the file

### Step 2: Place the skill in your Claude skills directory

Copy the `pm-interview-coach/` folder into your Claude user skills directory:

```
/mnt/skills/user/pm-interview-coach/SKILL.md
```

### Step 3: Use it in Claude

Once installed, Claude will automatically use this skill when you:
- Share a PM interview answer and ask for evaluation ("evaluate my answer", "how did I do?")
- Ask for a model answer to a product sense question
- Ask Claude to coach you on a specific dimension (segmentation, problem framing, etc.)

#### Example prompts to get started

```
"Here's my answer to 'How would you improve Spotify?' — can you evaluate it?"

"Generate a model answer for 'How would you improve Google Maps?'"

"Score my product sense answer and tell me where I'm weakest."
```

---

## Requirements

- Claude with skills/user directory support (e.g. Claude Code or a configured Claude environment)
- The `references/model-answers.md` file referenced in the skill is optional — the skill works without it, but adding your own model answer examples will improve coaching quality

---

## Contributing

Feel free to fork and add your own skills. PRs welcome.
