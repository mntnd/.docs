# TL;DR

* Forever maintained software. Untill we all die.
* All lanugages. All platforms. All frameworks.
* Maintenance priorities: 1 - security fixes, 2 - compatibility fixes, 3 - bug fixes, 4 - enhancements, 5 - new features.
* Only the first priority is guaranteed.
* Maximum automation.
* New project incubation happens after the project meets a number of conditions.

# What is mntnd?

An organisation aiming to maintain its software forever. At least ensure there are no security issues. Release vulnerability patches as fast as possible.

# How we gonna achieve that?

By automating as much as possible. Detect vulnerabilities in sub-dependencies - update them automatically, publish new package version.

If vulnerability found in the software itself - do everything possible to release a **non breaking** version of the software. We expect that the software package consumers would auto-update to the newest version by doing a non-breaking dependency upgrade.

We have 5 priority levels:

1. Security fixes - guranteed.
2. Compatibility fixes - not guranteed, but high priority. Often you can't fix a vulnerability without applying compatibility fixes.
3. Bug fixes - not guaranteed, medium priority. We would encourage companies to pay for this or volunteers to supply patches.
4. Enhancements - not guaranteed, low priority. Enhancement is an software update which does not fix this the software itself, like dependency upgrades.
5. New features - not guaranteed, not a priority. We can do this for money or do it yourself reliably.

# What's the difference from Node.js [pkgjs](https://github.com/pkgjs) organisation?

They are non commercial. Not much results in couple of years time. See the [article](https://medium.com/@nodejs/call-to-action-accelerating-node-js-growth-e4862bee2919) which sparkled the pkgjs. Quote:

> MQTT.js is another good example which is used by AWS, Microsoft, and IBM, however the maintainers have trouble in keeping up with the issues (110 and counting) while implementing new features.

It feels like enterprises (like IBM) effort to get more out of voulnteer developers and not paying for it. We don't see this as a viable effort.

Whereas, we intend to do it for money. Our main focus would be the software mostly used in interprises. We would like to win their trust by promising forever security.

Here is another quote from the same article:

> These packages are often downloaded millions of times per month, however they sit in very deep dependency trees and the community expects that they just work: no one is interested in maintaining them. As we accelerate the pace of change with more up to date V8 versions in Node.js, easier **vulnerability** reporting, and more automated **security auditing** this just adds to the burden on the package maintainers.

# What "mntnd" stands for?

The word "**m**ai**nt**ai**n**e**d**" without all the vowels - mntnd.
