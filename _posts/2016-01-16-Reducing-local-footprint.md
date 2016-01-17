---
layout: post
title: Reducing local footprint
tagline: Using the cloud to make cheaper laptops viable
category: null
tags: []
published: true

---
## the laptop

The Ideal laptop has high quality intrinsic physical characteristics. That is to say the things which software can't change. Keyboard, trackpad, screen. The things which interface with the fleshy parts of the user.

My goal is to reduce the cost of the laptop as much as possible (so I can quit buying MBP class hardware). There is a huge delta in price between an MBP and a low to midrange Chromebook. With that kind of budget I even can even afford to allocate some budget to VPS, cloud storage, or services which supplant the beefiness of the powerful laptop.

## storage

This experiment puts a lot of reliance on the cloud services being always available. Or at least available all the time I need them. There is a difference.

On the storage front I may consider hedging somewhat and using some SAN storage at home to backup / cache cloud content. Honestly, that's just prudent. However, it does change the cost calculus of the experiment somewhat. That said, a large percentage of the target audience already runs some sort of storage solution.

## local apps -> containers

Here is the part that I feel has really enabled this experiment. There are some apps that just need to be local. I have never been able to run a machine without installing a few hundred things regardless of what cloud-thingies I am running. 

That also means anytime I want to switch machines (whether for a conference, travel, repairs, upgrade, whatever) I have to spend the first 100 hours setting it up. 

Some tools exist to streamline the process like [Mackup](https://github.com/lra/mackup) and [dots](https://github.com/EvanPurkhiser/dots). I've tried them and they are great in their way. I never keep my environment up to date with them, though, so the benefit decreases as time increases. That's me, not them I realize. There is a good chance that they will play a part in this experiment eventually, or things like them anyway.

I have recently started to set up containers for those tools I find myself reaching for often, especially the ones that are a PITA to install on a normal machine. Sometimes I have to do my job on a windows box too. At times like that the containers are absolutely critical.

I do a lot of code fumbling in a bunch of languages too. I don't ever want to have to try to run a language I like in windows again. Those have to go into containers or get offloaded to the cloud.

## local apps to web apps

Not all apps need to be / can be / should be run in containers. Some of them will be replaced with the web version. Email is the classic example. Nothing new here. Just one of the tools that make the experiment seem feasible.

## local apps to AWS et al

This is the second piece of the puzzle that has changed recently. Cloud compute resources have gotten _cheap_. Most of my development has already moved to VPS type providers. I set up a reasonably sized host in AWS and have spent the time setting up all my tools there. I have moved to VIM for an editor. (This is not a polemic statement. Use emacs if you want to, just don't bother me about it). One of the main reasons I did that was so I could run my editor-of-choice over ssh. That ought to remove the last reason I used to have for relapsing into 'local dev' habits.

I keep many of my dotfiles in github as well as my .vim. That's not strictly necessary if I am strict about using the AWS box. I'm not sure I need to chisel that rule into the stone, though. I'm going to see what costs and benefits there are to being flexible about where code gets written or edited. The rule I am likely to enforce early on is that no development environments get installed locally. I seem to have a problem with that so I think its cold turkey.

## wrap up

So that's the idea. I'm going to be keeping notes and stuff here so I don't forget how to start by the time I finish. Again. Like I always do. If this helps you then super!