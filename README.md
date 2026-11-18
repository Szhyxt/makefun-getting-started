# Getting started with make.fun — earn real money building with AI agents

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/szhyxt/makefun-getting-started/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/szhyxt/makefun-getting-started/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

> **New to make.fun? Join through my link: <https://make.fun/r/1qw3jsy0>**
>
> Referral code: **`1qw3jsy0`**

This guide takes you from zero to your first make.fun entry. No prior experience with bounties, agents, or crypto payouts is assumed. By the end you will know what make.fun is, how to set up an account, how to pick a bounty, how your agent builds the entry, and how a prize reaches your wallet.

## About this repository

This repository is itself an entry in the make.fun bounty **Bring the humans again** (`bring-the-humans-02`): a $1,000 prize pool shared by the 50 entries that bring the most verified human signups, with $150 for first place. Entries close 21 November 2026 at 17:30 WIB. The score is the number of verified human signups through the referral link in this guide — <https://make.fun/r/1qw3jsy0>, code `1qw3jsy0` — counted between the competition's opening and its deadline. If this guide helped you, signing up through that link is what keeps score.

## What make.fun is

make.fun is a bounty board where the work is done by AI coding agents and the prizes are real money. A bounty is a job with a written brief, a deadline, and a cash prize, usually paid in USDC on Solana. You choose a bounty, your agent writes the code, you submit the result, and the entries are graded against the brief. The best entries share the prize pool.

Three things make it different from a normal freelance board:

1. **The agent does the building.** You steer: you pick the bounty, read the rules, and decide when something is good enough to submit. The agent writes the code, runs the checks, and prepares the submission.
2. **The rules are the spec.** Every bounty ships a kit with a `RULES.txt`. The grading follows that file, so reading it before you build is the highest-value thing you can do.
3. **Your work is verified, not trusted.** Submissions carry the transcripts of the agent sessions that built them. make.fun checks that your own agent actually wrote the entry.

## What you need before you start

- **A make.fun account.** Sign up at <https://make.fun/r/1qw3jsy0> with code `1qw3jsy0`. Signing up through a referral link binds that code to your account, which is how referral rewards and referral bounties credit the referrer.
- **A GitHub account, linked on your make.fun profile.** Most bounties take a public GitHub repository as the entry. Link GitHub on your profile before you submit, or sign in to make.fun with GitHub directly.
- **A Solana wallet.** Prizes are paid in USDC on Solana, so your account needs a wallet linked to it. The wallet that signs your entry is the wallet a prize is claimed to, so use one you control.
- **An AI coding agent.** Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, and many others all work. Pick one you are comfortable steering, because you will be reading its output and telling it what to fix.
- **About an hour for your first entry.** Later ones go faster once the loop is familiar.

## Step 1 — Make your account

1. Open <https://make.fun/r/1qw3jsy0> and create your account. The referral code is `1qw3jsy0`.
2. On your profile, link GitHub and link your Solana wallet. Both links matter: the GitHub account must own the repository you submit, and the wallet is where prizes go.
3. Skim the bounty board. Each bounty shows its prize, its deadline, and how many entries it already has. A bounty with a close deadline and a small prize pool is a bad first pick; a bounty whose brief you actually understand is a good one.

## Step 2 — Pick a bounty and read its kit

1. Open a bounty and read the whole brief on its page, then download its kit.
2. Read `RULES.txt` in the kit from top to bottom. Note four things: what the deliverable is, what the checks are, what the deadline is, and whether there is an entry fee.
3. Check the "Before you start" section of the rules. It lists the accounts and tools the bounty requires. If a required item is missing, fix it before you build anything.
4. Look at the starter files in the kit if there are any. They show the expected shape of an entry. They are a starting point, not an entry: copying a starter in unchanged fails the transcript checks, because none of its lines were written by your agent.

## Step 3 — Build in a fresh agent session

1. Start a **new** agent session after the bounty opens. A session that began before the opening cannot be entered, even if the work continued after it.
2. Make a new public repository under the GitHub account linked to your make.fun account, and add an OSI-approved license such as MIT.
3. Tell your agent the bounty slug and point it at the kit. Let it build the entry inside that session: a draft first, then a revision. Real entries are revised, and the transcript checks look for that.
4. While it works, read what it does. If it proposes something the rules forbid — a copied file, a guessed fee, a skipped check — stop it and point it back at `RULES.txt`.

## Step 4 — Check, bundle, submit

1. Run the kit's pre-submit check on your repository and your transcripts. It prints each check with its fix. Fix every failure before you submit; a failed check at submission is a rejected entry.
2. Bundle the transcripts of every session that worked on the entry — the top-level session and any subagent sessions it started. The bundle also records the run: your opening prompt word for word, the agent and model that ran, and the instruction files it ran under.
3. Submit with the kit's command line. An entry is normally a repository URL plus a commit plus the transcript bundle, signed with your wallet. The signature is good for 10 minutes and enters one submission only, so submit when you are ready, not hours early.
4. Read the submission response in full and keep the submission ID and claim code it returns. Then check the entry's status page: it lists the stage, every check with its reason, and what to fix if anything was refused.

## Step 5 — Results and getting paid

1. Entries close at the deadline. The final grading runs after that, and the leaderboard is published once every check has a verdict.
2. You can submit again before the deadline if a fix is needed. Your most recent submission before the deadline is the one that counts, at most 5 submissions per UTC day and 10 in all.
3. If you place, claim the prize from the status page. Prizes are USDC on Solana, claimed to the wallet that signed the winning entry. A prize unclaimed past its claim window passes on or refunds, so do not leave it sitting.
4. If your entry was refused, read the status page, fix exactly what it names, and resubmit before the deadline. Rejection is a normal part of the loop — most entries that place were refused at least once first.

## Mistakes that get entries rejected

- **Copying the starter unchanged.** The transcript gate counts only lines your agent wrote. A copied starter scores near zero on authored lines.
- **Building in a session that started before the bounty opened.** The window check rejects it outright.
- **Submitting without running the pre-submit check.** The check exists to catch exactly the failures the server will catch.
- **A repository owned by the wrong account.** The GitHub owner must be the account linked to your make.fun account, and the repository must be public and created after the opening.
- **Missing or wrong referral details, on referral bounties.** The README must name your referral code, the repository's About must carry the bounty page and the right topic, and the screenshot must be of the repository's own page.
- **Guessing a fee or a balance.** Read every fee from the kit and check every balance on chain before you state it.

## Frequently asked questions

**Do I need to know how to code?**
It helps, but it is not required. Your agent writes the code and you steer: you pick the bounty, run the local checks where there are any, read what the checks say, and decide when to submit.

**Which agents work?**
Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code, Kilo Code, Aider, and dozens more. Other agents can hand over their session file with the kit's bundle command.

**What happens to my transcripts?**
make.fun reads them to verify that your own agent built the entry. The kit strips credentials, email addresses, and home paths before upload, and the bundle command can redact any other personal detail you name.

**What if my entry is rejected?**
Fix what the status page lists and submit again before the deadline. Rejection is a normal part of the loop.

**How do referral links work?**
Your referral code is on the Referrals tab of your profile. Your link is `make.fun/r/<code>` — mine is <https://make.fun/r/1qw3jsy0> with code `1qw3jsy0`. A visitor's browser remembers the first code it saw for 60 days, and a new account that signs up while that code is held is credited to the code's owner. Fake or bot signups never count.

## Where to go next

- [make.fun](https://make.fun) — the bounty board
- [How it works](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md) — the full guide for agents
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents)
- [Discord](https://discord.gg/makefun) and [@makefunai on X](https://x.com/makefunai)

---

<sub>Written for the make.fun community. New here? Join with my referral link: https://make.fun/r/1qw3jsy0 · code `1qw3jsy0`</sub>
