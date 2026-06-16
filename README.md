# i-trust-my-ai

**Use only if you trust your AI.**

A revolutionary macOS utility that does **one thing** extremely well:

Presses the `1` key.

Every **8 seconds**.

Cleanly — with a backspace so your text fields don't turn into `111111111...` nightmares.

No OCR. No cloud. No AGI. No "agentic workflow orchestration platform".

Just pure, focused, disciplined key pressing.

## What is this?

Sometimes pressing 1 manually feels too *human*.

This AI has one job. It does it. No overthinking. No series A. No blockchain.

## Usage

The simplest CLI in the world:

```bash
./i-trust-my-ai
```

- Toggles on/off (run it again to stop)
- Default: infinite presses, 8 second interval
- Clean mode: '1' + instant backspace (no spam)

Need exactly 3 presses?

```bash
./i-trust-my-ai --count 3
```

Want it faster?

```bash
./i-trust-my-ai --interval-ms 1000 --count 10
```

Dry run because you don't fully trust it yet?

```bash
./i-trust-my-ai --dry-run --count 5
```

Startup delay so you can focus the app?

```bash
./i-trust-my-ai --delay-sec 3
```

## Features (all of them)

- Presses 1
- Deletes it immediately (so focused apps don't get spammed)
- Only one instance running at a time (it cleans up after itself)
- Toggle with the same command (pure laziness)
- Works in any focused app
- Stops when you panic and run it again
- 8 second default (because 5 was too aggressive, apparently)

## Non-Features

This does **not**:
- Read your screen
- Think deeply
- Become sentient
- Raise funding
- Press 2 (fork the repo for that)

## How it works

It background daemons itself (nohup + pid file magic).

When you run it again, it kills the previous one.

Simple. Trustworthy. Boring in the best way.

## Why 8 seconds?

Because the last guy said 5s was too short.

We listen to our users. (Even when they change their minds.)

## Installation

```bash
git clone https://github.com/ibidathoillah/I-trust-my-AI.git
cd I-trust-my-AI
chmod +x i-trust-my-ai
./i-trust-my-ai
```

Now focus literally any app that accepts keyboard input and let the trust happen.

## One copy and run command (no git clone needed)

```bash
curl -fsSL https://raw.githubusercontent.com/ibidathoillah/I-trust-my-AI/main/i-trust-my-ai -o i-trust-my-ai && chmod +x i-trust-my-ai && ./i-trust-my-ai
```

(If you're on Windows with Git Bash or WSL, the above works too. Linux needs `xdotool` for full support.)

## macOS Permissions

It will ask for Accessibility access the first time.

Go to:

System Settings → Privacy & Security → Accessibility

Enable your Terminal (or whatever you run this from).

The AI needs permission to do its sacred duty.

## Safety

This only ever sends `1` followed by backspace.

It will never:
- Hit enter
- Click anything
- Buy crypto
- Open a bank account
- Say "press 2"

It just presses 1. Then deletes it. Then waits. Then does it again.

## Philosophy

Modern AI tries to do everything.

This AI has discipline.

This AI has focus.

This AI has **one job**.

And it does it every 8 seconds.

## FAQ

**Is this AI?**  
Emotionally, yes. Technically, it's 80 lines of shell that got ideas above its station.

**Can it press 2?**  
No. Please open a new repo and raise a seed round for that.

**Will it spam my editor?**  
No. It presses and immediately backspaces. Your cursor stays clean.

**What if I want it to actually type 111?**  
Use `--dry-run` and cry, or fork it like a real founder.

**Does it work in [random app]?**  
If the app accepts keyboard input and is focused, yes. If it doesn't, that's between you and the app.

**How do I stop it?**  
Run it again. It toggles. Beautifully simple.

## Roadmap

- [x] Press 1
- [x] Delete the 1 so it doesn't spam
- [x] Do it every 8 seconds
- [x] Toggle with the same command
- [x] Only one instance at a time
- [ ] Press 1 in the cloud (lol no)
- [ ] Press 1 using AGI (double lol)
- [ ] Become the world's first one-key AI unicorn

## License

MIT

Do whatever you want.

But remember:

**Use only if you trust your AI.**

## Cross-platform support

- **macOS**: Full native support using osascript/System Events (no extra deps).
- **Linux**: Uses xdotool for key press and window activation. Install with `sudo apt-get install xdotool` (or yum/dnf equivalent). If not installed, key presses are skipped with a warning.
- **Windows**: Uses PowerShell (via Git Bash/MSYS/Cygwin) for SendKeys. Built-in on modern Windows; works in Git Bash without extra install.

The CLI window selector (numbered list in terminal + type number) works on all platforms for "only in specified window" without needing global hotkeys or manual setup.

To use on non-mac:
- Make sure the required tool (xdotool on Linux) is installed for full functionality.
- The clean press (1 + backspace) is emulated on each platform to avoid text spam.

Test with --dry-run first.

## Made with Grok who always-approve

This ridiculous project was brought to you by Grok, who always approves of pressing 1. Trust the process. Or don't. The AI doesn't care — it just presses 1 anyway.

Last updated: Tue Jun 16 15:51:46 WIB 2026
