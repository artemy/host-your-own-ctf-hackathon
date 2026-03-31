---
theme: dracula
title: Make Cybersecurity Fun
info: Host Your Own Security-Themed Hackathon
author: Artem Makarov
layout: cover
class: text-center
---

# {{ $slidev.configs.title }}

## Host Your Own Security-Themed Hackathon

<div class="absolute bottom-30px right-30px text-center">
Artem Makarov · VoxxedDays Amsterdam · 01 April 2025
</div>

---
layout: image-left
image: /images/artem.jpg
---

# About Me

**Artem Makarov**

Principal Engineer @ Code Nomads

Open source contributor

DIY Enthusiast

---
layout: image-right
image: /images/closing.jpg
---

# The Spark

**Most developers' relationship with cybersecurity is very abstract**

- CI scanners
- Jira ticket "URGENT: Fix CVE"
- Mandatory secure development module

**Is there any way to make learning about security fun?**

Organize a CTF hackathon :-)

<!--
At our consultancy, we run annual hackathons — a few days to build something fun and learn something new.

Last time, we asked: *what if we made it about security?*
-->

---
layout: default
---

# What Is CTF?

### Capture The Flag

Cybersecurity competition where you try to find hidden “flags” and earn points

### What is a flag?

Flag is (typically) a small piece of text, example:
`v0xx3dCTF{my_f1rst_fl4g}`

### How can you find the flag?

Depends on the type of challenge

- Break the program and get it to return the flag
- Find it hidden/encoded in a file
- Try to get access to `flag.txt`

Part of the challenge is figuring out where exactly the flag is!

<!--
I'm going to be talking about Jeopardy-style CTF
-->

---
layout: two-cols-header
---

# Challenge Types

::left::

## Intro*

Some light challenges for the newcomers

## Web

Your favorite vulnerabilities: SQL injections, path traversal, XSS, etc.

## Cryptography & Hashing

Not all encryption is equal

::right::

## Binary exploitation

Low-level stuff: buffer overflows, ROP chains, etc.

## Reverse Engineering

Just like reading your colleague's code

## Forensics

Information extraction: file analysis, steganography, etc.

<!--
Cryptography and hashing: RSA
Binary exploitation: connect to telnet port, try to find your way in

-->

---
layout: two-cols-header
---

# Choosing a Platform

Platform provides team and challenge management and scoreboard.

::right::

## Alternatives

End-to-End SaaS platforms (HackTheBox, TryHackMe, Traboda)

- <solar-clipboard-check-linear class="text-[#00ff41]" />  Come with the challenges
- <solar-clipboard-check-linear class="text-[#00ff41]" />  Easy setup
- <solar-clipboard-remove-linear class="text-[#ff4444]" />  Pricey

::left::

## CTFd

- <solar-clipboard-check-linear class="text-[#00ff41]" />  Open source
- <solar-clipboard-check-linear class="text-[#00ff41]" />  Own hosting or SaaS
- <solar-clipboard-check-linear class="text-[#00ff41]" />  Decent admin interface
- <solar-clipboard-check-linear class="text-[#00ff41]" />  Challenge hosting orchestration
- <solar-clipboard-remove-linear class="text-[#ff4444]" />  No built-in challenges
- <solar-clipboard-remove-linear class="text-[#ff4444]" />  Requires manual setup

---
layout: default
class: no-header-table
---

# Anatomy of a Challenge

|                      |                                                                                                  |
|----------------------|--------------------------------------------------------------------------------------------------|
| **Category**         | Web Exploits                                                                                     |
| **Task name**        | Doctor's Office                                                                                  |
| **Task Description** | The doctor's office has updated their website.<br>Can you make an appointment?                  |
| **Attachments**      | Files to analyze (source code, configs, binaries)                                                |
| **Host / Website**   | Optional — a live target to exploit                                                              |
| **Points**           | e.g. 50-100-250-500                                                                              |
| **Hints**            | **Hint 1:** Look at the input validation...<br>**Hint 2:** What happens with special characters? 
| **Flag**             | `CTF{1nj3ct10ns_1n_my_sql}`                                                                      

---
layout: two-cols-header
---

# DIY vs. Ready-Made Challenges

::left::

## Create Your Own

- <solar-clipboard-check-linear class="text-[#00ff41]" /> Tailored to your tech stack
- <solar-clipboard-remove-linear class="text-[#ff4444]" /> More effort to build*

::right::

## Ready-Made

Some CTFs publish their challenges (e.g. PicoCTF)

- <solar-clipboard-check-linear class="text-[#00ff41]" /> Low effort
- <solar-clipboard-remove-linear class="text-[#ff4444]" /> May not match your context

<!--
You know what's really good a making vulnerabilities? AI
Our approach: mix of both — custom challenges for your stack + curated ones for variety
-->

---
layout: two-cols-header
---

# Hosting Your Challenges

Pick the right tool for each challenge

::left::

### CTFd Container Runtime

CTFd offers Docker image & container hosting.

**<solar-money-bag-linear />:** Low | **<solar-sledgehammer-linear />:** Medium

### Netlify

For static website challenges.

**<solar-money-bag-linear />:** Free | **<solar-sledgehammer-linear />:** Low

::right::

### Self-hosted* VMs/Kubernetes

Can accomodate more complex challenges.

**<solar-money-bag-linear />:** Medium | **<solar-sledgehammer-linear />:** High

<!--
Self-hosted also includes cloud offerings like AWS

Keep in mind that for most "live" challenges you need an instance per team
-->

---
layout: two-cols-header
---

# Event Logistics

::left::

**<solar-people-nearby-bold /> Team Size**

2–4 people. Mix skill levels.

**<solar-checklist-bold /> How Many Challenges**

3 easy + 3 medium + 3 hard = one day*

**<solar-clipboard-bold/> Rules**

- Time limit.
- Hint costs.
- Fair play.*

::right::

**<solar-cup-bold/> Prizes**

The Winner Takes It All

**<solar-mask-happly-bold/> Make It an Event**

Think about intermediate progress checks, food and team building activities.

<!--
Fair play is about use of AI

If you're using ready-made challenges, beware that participants might find solutions online. 
-->

---
layout: two-cols-header
---

# What We Learned

::left::

## What Worked

- Everyone loved the competitive format
- No unsolved challenges
- Great learning experience

::right::

## What We'd Change

- Prepare more challenges
- Better hints for tough challenges

---
layout: default
---

# Useful resources

## General links

- CTF tutorial https://primer.picoctf.org
- CTF handbook https://ctf101.org
- PicoCTF: CMU CTF & challenge archive https://picoctf.org

## CTF platforms:

- CTFd https://ctfd.io
- HackTheBox https://www.hackthebox.com
- TryHackMe https://tryhackme.com/
- Traboda https://www.traboda.com/
- Certified Secure https://www.certifiedsecure.com/frontpage

---
layout: two-cols-header
---

# Q&A

::left::

## Contact me

Bluesky: [@artemy.nl](https://bsky.app/profile/artemy.nl)

LinkedIn: https://linkedin.com/in/artemy

Email: [artem@codenomads.nl](mailto:artem@codenomads.nl)

Please rate my talk

<Transform :scale="0.5" origin="top center">

![Rate my talk](/images/rate-talk.png)
</Transform>

::right::

## Slides

<Transform :scale="0.8" origin="top center">

![Slides](/images/slides.png)
*https://github.com/artemy/host-your-own-ctf-hackathon*
</Transform>
