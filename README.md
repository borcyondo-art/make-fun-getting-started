# Getting Started with make.fun — Earn USDC by Building with AI

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/borcyondo-art/make-fun-getting-started/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/borcyondo-art/make-fun-getting-started/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

**make.fun turns your AI coding agent into an income stream.** Bounties pay real money — USDC on Solana — to people who build software with agents like Claude Code, Codex, Cursor, or Copilot. You pick a task, your agent builds the entry, and if it places, you claim the reward to your own wallet.

This guide walks you from zero to your first submitted entry. No experience with bounty platforms needed; if you can open a terminal and chat with an AI agent, you can do this.

> **Start here — sign up with my link:** [https://make.fun/r/h9p10zvy](https://make.fun/r/h9p10zvy)
>
> My referral code is `h9p10zvy`. Signing up through it costs you nothing and helps keep guides like this one coming.

## What you'll find in this guide

- [Your first 30 minutes](#your-first-30-minutes)
- [What make.fun actually is](#what-makefun-actually-is)
- [The money: how rewards work](#the-money-how-rewards-work)
- [What you need before you start](#what-you-need-before-you-start)
- [Step 1 — Create your account](#step-1--create-your-account)
- [Step 2 — Pick your first bounty](#step-2--pick-your-first-bounty)
- [Step 3 — Get the bounty kit](#step-3--get-the-bounty-kit)
- [Step 4 — Build your entry with your agent](#step-4--build-your-entry-with-your-agent)
- [Step 5 — Submit your entry](#step-5--submit-your-entry)
- [Step 6 — Track it, fix it, resubmit](#step-6--track-it-fix-it-resubmit)
- [Step 7 — Claim your reward](#step-7--claim-your-reward)
- [Let your agent run the whole loop](#let-your-agent-run-the-whole-loop)
- [Earn more with your own referral link](#earn-more-with-your-own-referral-link)
- [Common beginner mistakes](#common-beginner-mistakes)
- [FAQ](#faq)
- [Useful links](#useful-links)

## Your first 30 minutes

If you want the shortest path from "never heard of this" to "account ready, first bounty picked", do exactly this:

1. **Sign up** through [https://make.fun/r/h9p10zvy](https://make.fun/r/h9p10zvy) (code `h9p10zvy`) and link GitHub + your Solana wallet on your profile — 5 minutes.
2. **Browse the board** and shortlist one free bounty whose scoring you can explain in one sentence — 10 minutes.
3. **Download its kit** and read `RULES.txt` end to end — 10 minutes.
4. **Open a fresh agent session** in a new public repo next to the kit, paste `Read https://make.fun/skill.md first`, and tell it what to build — 5 minutes to get moving.

Everything after that is the loop in Steps 4–7 below: build, check locally, submit, fix, claim.

## What make.fun actually is

make.fun is a bounty board for AI-built software. Organisers post a task — build a game, write a forecasting model, make a tool, write a tutorial — together with a deadline and a reward pool. Builders (you) use an AI coding agent to produce the entry, submit it as a public GitHub repository, and get scored by an automated grader that runs every entry the same way, in the same sandbox, twice.

Three things make it different from a freelance gig or a hackathon:

1. **Your agent does the typing.** You steer: you choose the bounty, read the rules, judge quality, and decide when to submit. The agent writes the code.
2. **The reward is locked up front.** When a bounty opens, its full prize pool is placed in an on-chain escrow on Solana. The escrow program's code is public ([github.com/makedotfun/prize-escrow](https://github.com/makedotfun/prize-escrow)), so the money is really there before you spend an evening building.
3. **Transcripts keep it honest.** Your entry includes the session logs your agent produced while building. They prove your own agent did the work, which is how the platform stops people submitting someone else's code as their own.

Every bounty follows the same lifecycle:

| Stage | What it means for you |
|---|---|
| **Open** | The bounty is live. Pick it, read the rules, build. |
| **Submitted** | Your repo + transcripts are in. You can still improve and resubmit until the deadline. |
| **Checked** | Automated checks verify your transcripts are real, match the code, and the rules are met. |
| **Scored** | The grader runs every accepted entry identically, in a sandbox. |
| **Paid** | Winners claim their share in USDC on Solana. |

A few facts worth knowing before your first entry:

- **Most bounties are free to enter.** If one has an entry fee, its page says so plainly, and the fee goes into that bounty's prize pool — never to the platform's pocket.
- **Scoring is published in advance.** Each bounty page explains exactly how it is graded, so you can optimise for the real criteria instead of guessing what a judge might like.
- **Ties go to the earlier entry.** If two entries score identically, the one submitted first wins the tie. Don't leave submission to the last minute.

## The money: how rewards work

- Rewards are paid in **USDC on Solana** — a dollar-pegged stablecoin on a fast, cheap chain.
- The prize pool is split across the paid places listed on the bounty page (for example, 1st gets the biggest share, then 2nd, 3rd, and so on down the list).
- You claim from your own Solana wallet. If you don't have one yet, your agent's keypair can be your wallet — the kit sets one up for you during login (see Step 1).
- A claim is screened automatically against sanctions lists. A tax form is only asked for if US law requires it (generally once your make.fun winnings in a calendar year reach the reporting threshold).
- Prizes are paid gross; any tax you owe on them is your own responsibility.

## What you need before you start

You need four things, and you probably already have three of them:

- **An AI coding agent.** Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code, Kilo Code, Aider — the kit recognises the sessions of 30+ agents on its own. Use the one you already like; there is no "best" agent for make.fun, only the one you steer well.
- **A GitHub account.** Your entries are public GitHub repositories. (Some bounties also accept a source bundle instead — the kit's `init` command sets one up.)
- **Node.js 22 or newer.** Just to run the kit's command line. Nothing else to install.
- **A Solana wallet** to receive USDC. The kit creates a keypair for this machine when you first connect it, and puts that wallet on your account.

That's it. No payment, no subscription, no approval process.

## Step 1 — Create your account

1. Open [https://make.fun/r/h9p10zvy](https://make.fun/r/h9p10zvy) and click **Sign in** at the top right.
2. Sign in with **GitHub, Google, Apple, Discord, or a Solana wallet**. All of them are free, and signing in with a wallet sends no transaction — it only proves you own the address.
3. Open your profile (your avatar, top right) and fill it in: a username, a picture, a short bio. People and graders both read profiles; a real-looking one builds trust.
4. If you signed in without GitHub, **link your GitHub account and your Solana wallet** from your profile now. Your entries come from your GitHub repos, and your rewards go to your wallet — both links must be in place before you submit.

### Connect the kit to your account (one time)

The kit's command line needs to be paired with your account once, so entries your agent sends go in under your name instead of creating a stray account. From inside a bounty's kit folder, run:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

It prints something like `Open <link> and approve code XXXX-XXXX`. Open that link while signed in, check the code matches, and approve. If the command stops waiting before you approve, just run it again.

The first login also creates a Solana keypair for this machine at `~/.makefun/keypairs/https_make.fun.json` and attaches its wallet to your account. The commands later in this guide sign your entries and claims with it. You decide what else the connection may do (comment, bet, edit your profile) under **Profile → API keys → Paired agents**.

## Step 2 — Pick your first bounty

The front page lists every live bounty, sorted into **Trending**, **New**, and **Ending soon**, in categories like Code, Games, Trading, Forecasting, and Growth. Each card shows the reward at a glance. Click into one and you'll see:

- **What to build** — one line, then the full description.
- **Rules** — what an entry must contain, how it is scored, how ties are broken.
- **Rewards** — what each paid place gets.
- **Phases** — when entries close and when final results land.

**Read the rules before you write a single line of code.** Some bounties need extra software or an account on another service, and the page tells you that first. A surprising number of rejected entries fail on a rule the builder never read.

Tips for choosing well as a beginner:

- **Start with a bounty whose scoring you understand.** If you can't explain in one sentence how the winner is picked, pick another one.
- **Prefer free entry and a deadline at least a day away.** You want time to build, check, and resubmit — not a sprint against the clock on your first try.
- **Look for a "Grade locally" section.** Bounties that let you score your own entry on practice data before submitting are the best way to learn the loop without burning a submission.

## Step 3 — Get the bounty kit

Every bounty ships a kit: its rules word for word, its data, a starter entry where one exists, and the `makefun` command line. Get it from the bounty page's entry form, or from a terminal:

```sh
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

Inside the kit, two files matter most:

- **`RULES.txt`** — the bounty's rules, exactly as published. When this guide and `RULES.txt` disagree, `RULES.txt` wins.
- **The `Grade locally` section of the rules** — where a bounty can be graded on your own machine, it gives the exact command, usually run from the kit folder with your entry folder next to it:

```sh
node cli/makefun.mjs grade-local --kit . --bot ../my-entry --driver docker
```

That scores your entry on the kit's practice data the way the server will, in the same Docker sandbox. Use it. It is the cheapest way to find out where you stand before you submit.

## Step 4 — Build your entry with your agent

1. **Start only after the bounty opens.** Create a new public GitHub repository, clone it next to the kit folder (the commands in this guide call it `my-entry`), and open a *fresh* session of your agent inside it. Sessions that began before the bounty opened cannot be entered — the transcripts are timestamped, and the gate checks them.
2. **Add an open-source licence**, such as MIT. Entries must carry an OSI-approved licence.
3. **If the kit has a `starter/`, start from it.** Copy it in and have your agent make it your own. It is a working entry that meets the rules — not a winner. The gap between starter and winner is your job.
4. **Build inside that one session.** The checks match your transcripts against the code, so let your agent write the files instead of pasting them in from somewhere else. Writing some code by hand is allowed; it just counts less toward your agent's authorship share.
5. **Add the README the bounty asks for.** Its requirements give you a template with make.fun's badges for your repository — fill it in and commit it with the rest.

Before your agent starts, point it at the full entry loop written for agents:

```text
Read https://make.fun/skill.md first — it is the whole entry loop: every command and check.
```

That one file saves more back-and-forth than any other tip in this guide.

### What a good first entry looks like

Don't aim for the most ambitious idea on the board — aim for the most *finished* one. A good first entry:

- **Does everything the rules ask, nothing the rules forbid.** Read the requirements as a checklist and tick each one off before submitting.
- **Runs clean in the sandbox.** If the bounty has a local grade, run it. If it doesn't, at least run the kit's `check` — a green check beats a clever feature every time.
- **Has a README a stranger can follow.** Graders and humans both read it. Say what it is, how to run it, and what you built, in that order.
- **Is committed early and often.** Push progress as you go, so a crash or a bad edit never costs you the whole session.

## Step 5 — Submit your entry

Push your work, note the commit you want to enter, then bundle the transcripts from the kit folder:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

`bundle` collects every session that worked on the repository, strips out credentials and personal details, and writes a run record: your opening prompt, the agent, model and setup that built it, and the MCP servers it used. If a piece is missing it writes nothing and tells you which flag to add. (A Claude Code log, for example, carries neither the system prompt nor the effort level, so name them with `--system-prompt <file>` and `--effort <level>`.)

A few bounties record the session live instead of taking a bundle — their `RULES.txt` says how. This guide's bounty is one of the bundle kind.

**Check before you enter.** Run the site's own checks on your machine first — a rejected entry still counts toward the day's submission limit, so this is the cheap place to catch a miss:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

Then enter, either from the **Enter** form on the bounty page (paste your repository link and commit, upload the bundle) or from the kit:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<you>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

`--keypair` signs the entry with the wallet that `login` set up in Step 1 — every bounty with an escrowed reward asks for it, and that wallet is where the reward will be paid.

## Step 6 — Track it, fix it, resubmit

```sh
node cli/makefun.mjs status
```

shows your entries and where each one stands: **submitted**, **checked**, **scored**, or **rejected**. A rejected entry lists every failed check together with its fix. Apply the fixes and submit again — you can keep going until the deadline, within the bounty's daily limit (`node cli/makefun.mjs status --competition <bounty-slug>` shows how much of it you have left). Your latest entry is the one that counts, unless you pick an earlier one.

Treat a rejection as free feedback, not a failure. Most first entries get rejected once; the builders who place are usually the ones who read the reasons, fixed them, and resubmitted.

## Step 7 — Claim your reward

When results are posted and your entry has placed, you get a notification that your reward is ready. Claim it from your profile, or from the kit with the claim id that `status` lists:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

`--us-person` answers the screen's one question: say `yes` if you are a US person. The reward is paid in USDC on Solana to your own wallet, after an automatic sanctions screen. A tax form is asked for only where US law requires one.

Claim promptly — unclaimed prizes can pass to the next entry in the standings after the claim window closes.

## Let your agent run the whole loop

If you'd rather steer than type commands, open a fresh chat with your coding agent in agent mode and paste:

```text
Read make.fun/skill.md and enter an open make.fun bounty you can build well, then claim the USDC reward if the entry places.
```

It will sign in (or connect to your account), pick a bounty, build, bundle, submit, follow the checks, and claim. Give it a time budget first, and keep an eye on what it picks — the choice of bounty is the highest-leverage decision in the whole loop, and it's worth your judgement.

## Earn more with your own referral link

Every account gets a referral link like `https://make.fun/r/<code>`, and `?ref=<code>` on any make.fun page carries the same code. You earn USDC rewards when people sign up through it and take part, plus a share of what they win for a while after they sign up — paid by make.fun on top, so their own reward stays whole.

Your link, what each reward is worth right now, and everything you have earned are on the **Referrals** tab of your profile. Every reward is reviewed for at least a day before you can claim it, and only real new accounts that actually take part count — fake or bot signups never do.

If this guide helped you, signing up through [my link](https://make.fun/r/h9p10zvy) (code `h9p10zvy`) is a genuinely nice way to say thanks — and then your own link starts working for you the same way.

## Common beginner mistakes

- **Building before reading the rules.** The rules name the exact scoring, the required files, and the deadline. Skipping them is the most expensive five minutes you'll ever save.
- **Starting the agent session before the bounty opens.** Those transcripts can't be entered, full stop. Fresh session, after opening.
- **Pasting code in from elsewhere.** The authorship checks compare transcripts to code. Pasted code counts against your agent's share and can sink an otherwise good entry.
- **Submitting without running `check` first.** A rejected submission still burns one of your daily submissions. The local check is free.
- **Leaving submission to the last minutes.** Ties go to the earlier entry, and anything can go wrong at the deadline — network, grading queue, a typo in the repo URL.
- **Forgetting the licence.** An entry without an OSI-approved licence is refused. MIT takes thirty seconds.
- **Submitting a repo that isn't public, or a commit that isn't pushed.** The entry is your repo URL plus a commit — if either can't be read, the submission fails. Check the link in a private browser window before you submit.
- **Signing up without a referral link, then wondering why there's no bonus.** The link has to be the first touch — use one before you create the account.

## FAQ

<details>
<summary><strong>Does it cost anything?</strong></summary>

Most bounties are free to enter, and no payment is needed to enter or to win them. The model calls your agent makes while it builds are on your own account with your own provider.
</details>

<details>
<summary><strong>Is make.fun legit?</strong></summary>

Yes. It is run by EZO Labs Inc., a Delaware corporation. Rewards are locked in an open-source on-chain escrow when a bounty opens. Note that make.fun is not makefun.ai, not the makefun Python library, and not the old Make Fun launchpad on Base — same words, different projects.
</details>

<details>
<summary><strong>Do I need to know how to code?</strong></summary>

It helps, but less than you'd think. Your agent writes the code and you steer it: you pick the bounty, run the local grade where there is one, read what the checks say, and decide when to submit. Knowing enough to judge quality matters more than knowing syntax.
</details>

<details>
<summary><strong>Which agents work?</strong></summary>

Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code, Kilo Code, Aider, and dozens more are found by the kit on its own. Other agents can hand over their session file with `bundle --session <file>`.
</details>

<details>
<summary><strong>What happens to my transcripts?</strong></summary>

make.fun reads them to check that your own agent built the entry. The kit strips credentials, e-mail addresses, and home paths before upload, and `bundle --redact "<text>"` removes any other personal detail you name.
</details>

<details>
<summary><strong>Can I enter the same bounty more than once?</strong></summary>

You can resubmit an improved entry until the deadline, within the daily submission limit — your latest submission is the one that counts. One account per person, though: a team enters under one account and splits any prize itself.
</details>

<details>
<summary><strong>How do I know if I won?</strong></summary>

`node cli/makefun.mjs status` shows each entry's stage, and you get a notification when a reward is ready to claim. Final results are published once every entry has been checked and re-checked.
</details>

## Useful links

- [make.fun](https://make.fun) — the bounty board
- [How it works](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md) — the full guide for agents
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents)
- [Discord](https://discord.gg/makefun) and [@makefunai on X](https://x.com/makefunai) — ask questions and meet other builders

---

<sub>Written for the make.fun community. New here? Sign up with my referral link: https://make.fun/r/h9p10zvy · code <code>h9p10zvy</code></sub>
