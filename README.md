# Minecraft Server

## Goals
* maintain a private repo of configuration files
* collection of common:
  * Scripts
  * Files
  * mods specific to our community or client experience
  * Databases
  * NBT database store for safety
  * generic Dockerfiles for vanilla experiences
  * Specialized ansible playbooks for the base image

* Grocery List
1. Jar of Forge (1.19.2 collected thus far)
	a.Instance  that has been run once to generate eula.txt and set “eula” to true.
2. Jar of paper
3. Pre-gen minigame builds
   * Manhunt
   * Bedwars
   * Zombies
   * Escape rooms

## Vibe
   * Gotta have Game themes for the desktop if you’re gonna be in there editing
   * Hentai and anime themes work too☑☑☑☑☑☑☑☑☑☑☑☑☑☑☑☑☑☑

## Tools
* VS Code is literally a must have for editing minecraft files imho
* Java 8~latest (maybe not 8 anymore it depends on which packs we support)

## Timeline

Direct connection (ssh, ftp, vnc, rdp. Get to where we can do what we need to do.)
* ssh ☑
* ftp ☑
* vnc x needs addressed
* rdp ☑

## Admin tools
*(quickly launch applications and manage files from a client using an application*

* Get to where we can do what we need to do from one screen.)

## Web Interface
*upload, download, launch, and manipulate server from a web control panel. Get to where we can do what we need with completely server-sided tools.*

* Python and HTML5 to get off the ground

## my thoughts
```
Lots of “hosts” don’t do much more than offer you a thing to rent. I’m thinking of more like having an ecosystem of tools built around a community that can support itself. If we build the beginnings of infrastructure as code now we will later be more easily able to move into kubernetes and HA infrastructure

So as is the VM is a clone of a backup
We put that clone into prod and basically hand it out as of right now

But say we beef it up with some kind of workflow you double click a yaml file it opens in VS Code already, you open your files and on the side is your minecraft mods configuration directory – that sort of thing

From there you make that a “loadout” for this clone so now we have two pieces of infrastructure, the clone, then this loadout that is written out by ansible

We can host any of our individual pieces on our own infra in MySQL databases or just in storage, and get at it with Python or anything else
```