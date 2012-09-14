# Minecraft Server Manager [![Build Status](https://secure.travis-ci.org/marcuswhybrow/minecraft-server-manager.png?branch=master)](http://travis-ci.org/marcuswhybrow/minecraft-server-manager) [![Flattr this git repo](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=marcuswhybrow&url=https://github.com/marcuswhybrow/minecraft-server-manager&title=Minecraft%20Server%20Manager&language=en_GB&tags=github,minecraft,bukkit,init,init.d,linux,ubunut&category=software) 

A single init script which makes running multiple Minecraft/Bukkit servers easier for us admins.

## Quick Debian Install

Install MSM on a debian box using my install script:

    wget -qO- http://git.io/A5s1tQ | sh

Have a read of the script first if calms you: http://git.io/A5s1tQ

## Getting Started

* [Install][install] MSM on your box.
* [Visit the docs][docs] for help with getting started.
* Fork and contribute your own modifications.
* Not a coder? [Post an issue][issues] with your idea for MSM instead.
* Read the [changelog][changelog] to get a picture of how MSM has evolved over time.

MSM is released under the GPLv3 licence, which is included in the repository [here][licence]. I'm open to suggestions where licencing is concerned.

## Features

As well as starting, stopping and restarting MSM has the following features:

* One script handles multiple servers, run two or more servers on one machine.
* Can create and start new servers with a single command, downloads the jars for you.
* Periodically makes [WorldEdit snapshot][we-snapshot] compatible backups of your worlds.
* Backup the entire server directory for complete protection.
* Load world's into RAM for faster access (reduces lag).
* Easily configurable global defaults, with per server overrides if needed.
* Apply server commands to one, multiple, or all servers in one go (useful for whitelisting a player on all servers.)
* Tab completion for all commands, makes everything faster and getting started a breeze.
* Keep server logs organsied by periodically "rolling" them.
* Organises jar files into groups (such as minecraft and craftbukkit) and links each server to a single jar. Includes automated download of new versions.
* Plethora of in-game commands (whitelist, blacklist, operator, gamemode, kick, say, time, toggledownfall, save)
* Send commands straight to the server via the command line.

## Support

1. If you find a problem with MSM and you think the problem is one that requires changing code [submit an issue][issues] via GitHub.
2. If you otherwise have a problem, question or suggestion you can email me directly at msm@marcuswhybrow.net.


## Upcomming features

* **QuickBackup:** If you store your backups non-locally (maybe on a NAS), QuickBackup optionally creates a backup locally for speed, and then moves it after your players are building again! My initial testing shows a 54 second network backup confaltes to 23 seconds of in-game time.
* **Restore:** Roll-back to an old world or whole server backup automatically.


## Versioning

MSM uses semantic version numbers to better describe what code one might have installed, and indicate backwards incompatible changes.

Releases will be numbered with the follow format:

`<major>.<minor>.<patch>`

And constructed with the following guidelines:

* Breaking backward compatibility bumps the major (and resets the minor and patch)
* New additions without breaking backward compatibility bumps the minor (and resets the patch)
* Bug fixes and misc changes bumps the patch

For more information on SemVer, please visit http://semver.org/.


## Acknowledgements

This code grew out of an old version of [Ahtenus' Minecraft Init Script][ahtenus-minecraft-init].

[we-snapshot]: http://wiki.sk89q.com/wiki/WorldEdit/Snapshots
[ahtenus-minecraft-init]: https://github.com/Ahtenus/minecraft-init
[docs]: http://marcuswhybrow.github.com/minecraft-server-manager/docs/
[install]: http://marcuswhybrow.github.com/minecraft-server-manager/docs/installation.html
[changelog]: https://github.com/marcuswhybrow/minecraft-server-manager/blob/master/CHANGELOG.markdown
[licence]: https://github.com/marcuswhybrow/minecraft-server-manager/blob/master/LICENSE.markdown
[issues]: https://github.com/marcuswhybrow/minecraft-server-manager/issues