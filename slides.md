---
theme: dracula
title: Make Cybersecurity Fun
info: Host Your Own Security-Themed Hackathon
transition: slide-left
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
image: images/artem.jpg
---

# About Me

**Artem Makarov**

Principal Engineer @ Code Nomads

Open source contributor

DIY Enthusiast

---
layout: image-right
image: images/closing.jpg
---

# The Spark

How to make cybersecurity fun and engaging for developers?

Organize a hackathon :-)

<!--
Developers mostly hear about cybersecurity in the abstract — but rarely get hands-on experience.

We wanted to change that.
Make it engaging, fun and memorable.

So we organized a CTF hackathon

-->

---
layout: default
---

# What Is CTF?

## Capture The Flag

Cybersecurity competition where you try to find hidden “flags” and earn points

## What is a flag?

Flag is (typically) a small piece of text, example: 
`v0xx3dCTF{my_f1rst_fl4g}`

## How can you find the flag?

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

Weak crypto, poor secrets

::right::

## Binary exploitation

Assembly or Bust: buffer overflows, ROP chains, etc.

## Reverse Engineering

You get a binary and need to understand how it works

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

::right::

## Alternatives

End-to-End SaaS platforms (HackTheBox, TryHackMe, Traboda)

- <solar-clipboard-check-linear class="text-green-700" />  Come with the challenges
- <solar-clipboard-check-linear class="text-green-700" />  Easy setup
- <solar-clipboard-remove-linear class="text-red-700" />  Pricey

::left::

## CTFd (https://ctfd.io)

- <solar-clipboard-check-linear class="text-green-700" />  Open source
- <solar-clipboard-check-linear class="text-green-700" />  Own hosting or SaaS
- <solar-clipboard-check-linear class="text-green-700" />  Decent admin interface
- <solar-clipboard-check-linear class="text-green-700" />  Challenge hosting orchestration
- <solar-clipboard-remove-linear class="text-red-700" />  No built-in challenges
- <solar-clipboard-remove-linear class="text-red-700" />  Requires manual setup

<!--
Platform to:
- host challenges
- manage teams
- track scores
-->

---

# Anatomy of a Challenge

|                                                                            |                                                                                                  |
|----------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
| <solar-alt-arrow-right-bold class="text-green-700" /> **Category**         | e.g. Web Exploits                                                                                |
| <solar-alt-arrow-right-bold class="text-green-700" /> **Task name**        | Doctor's Office                                                                                  |
| <solar-alt-arrow-right-bold class="text-green-700" /> **Task Description** | The doctor's office has updated their website. Can you make an appointment?                      |
| <solar-alt-arrow-right-bold class="text-green-700" /> **Attachments**      | Files to analyze (source code, configs, binaries)                                                |
| <solar-alt-arrow-right-bold class="text-green-700" /> **Host / Website**   | Optional — a live target to exploit                                                              |
| <solar-alt-arrow-right-bold class="text-green-700" /> **Points**           | e.g. 50-100-250-500                                                                              |
| <solar-alt-arrow-right-bold class="text-green-700" /> **Hints**            | **Hint 1:** Look at the input validation...<br>**Hint 2:** What happens with special characters? 
| <solar-alt-arrow-right-bold class="text-green-700" /> **Flag**             | `CTF{1nj3ct10ns_1n_my_sql}`                                                                      

---
layout: two-cols-header
---
# DIY vs. Ready-Made Challenges

::left::

## Create Your Own

- <solar-clipboard-check-linear class="text-green-700" /> Tailored to your tech stack
- <solar-clipboard-remove-linear class="text-red-700" /> More effort to build

::right::

## Ready-Made

Some CTFs publish their challenges (e.g. PicoCTF)
- <solar-clipboard-check-linear class="text-green-700" /> Low effort
- <solar-clipboard-remove-linear class="text-red-700" /> May not match your context

<!--
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
- All challenges were completed
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

![Rate my talk](./images/rate-talk.png)
</Transform>

::right::

## Slides
<Transform :scale="0.8" origin="top center">

![Slides](./images/slides.png)
*https://github.com/artemy/host-your-own-ctf-hackathon*
</Transform>
