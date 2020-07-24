# TL;DR

* Forever maintained software. Untill we all die.
* We take existing but deprecated or abandoned software and promise to keep it forever secure by regularly patching it.
* All lanugages. All platforms. All frameworks.
* Maintenance priorities: 1 - security fixes, 2 - compatibility fixes, 3 - bug fixes, 4 - enhancements, 5 - new features.
* Only the 1-st priority is guaranteed.
* We'll try to automate as many processes as possible.
* We accept projects after it meets a number of conditions.

# What is mntnd?

An organisation aiming to maintain its software forever. At least ensure there are no security issues. Release vulnerability patches as fast as possible.

# How we gonna achieve that?

## Automation, automation, automation

By automating as much as possible. Detect vulnerabilities in sub-dependencies - update them automatically, publish new package version.

## Non-breaking releases

If vulnerability found in the software itself - do everything possible to release a **non breaking** version of the software. We expect that the software package consumers would auto-update to the newest version by doing a non-breaking dependency upgrade.

## Our priority levels

We have 5 priority levels:

1. Security fixes - guranteed.
2. Compatibility fixes - not guranteed, but high priority. Often you can't fix a vulnerability without applying compatibility fixes. Otherwise, we expect donations.
3. Bug fixes - not guaranteed, medium priority. We would encourage companies to pay for this or volunteers to supply patches.
4. Enhancements - not guaranteed, low priority. Enhancement are neither bugs nor features. E.g. dependency upgrades.
5. New features - not guaranteed, not a priority. We can add a feature for money, or you can do it yourself in a reliable fashion (unit tests, security review, etc).

## 0-inbox GitHub issues

We promise to keep 0-inbox approach in each project. Meaning, that number of open issues will be always near 0 in each project. And how are we going to achieve that?

## Issue triaging

Every issue gets triaged ASAP. A corresponding issue label is put on each.

* If you open a new GitHub issue and ask for a **new feature** - the issue get closed ASAP, but left open for any following discussions.
* Same fore **enhancements**.
* Same for **bugs**. (Yep. This is intentional. Our focus is security.)
* Same for **compatibility** problems.
* **Security** issues will be kept open until the patch is released.

You can search GitHub issues by labels. We encourage you to do so if, for example, you need to find a feature request.

# How mntnd is different from Node.js [pkgjs](https://github.com/pkgjs) organisation?

Pkgjs have similar goal as mntnd. Keep popular packages supported.

See the [article](https://medium.com/@nodejs/call-to-action-accelerating-node-js-growth-e4862bee2919) which sparkled the pkgjs. Quote:

> MQTT.js is another good example which is used by AWS, Microsoft, and IBM, however the maintainers have trouble in keeping up with the issues (110 and counting) while implementing new features.

It feels like enterprises (like IBM) effort to get more out of voulnteer developers and not paying for it. We don't see this as a viable effort. Pkgjs is non commercial. Thus, there is not much outcome in couple of years time.

Whereas, we intend to do it for money. Our main focus would be the software mostly used in interprises. We would like to win their trust by promising forever security.

Here is another quote from the same article:

> These packages are often downloaded millions of times per month, however they sit in very deep dependency trees and the community expects that they just work: no one is interested in maintaining them. As we accelerate the pace of change with more up to date V8 versions in Node.js, easier **vulnerability** reporting, and more automated **security auditing** this just adds to the burden on the package maintainers.

Also, pkjs have quite strict rules for everything. Whereas we are going to be as agile (flexible) as possible to cut times and lower various barriers.

# You say Node.js, but what about Python, Go and others?

We embrace all languages, for all platforms, all frameworks, all operating systems, all environments, etc.

It's just the Node.js is our first focus, because it needs us the most at this time.

# What "mntnd" stands for?

The word "**m**ai**nt**ai**n**e**d**" without all the vowels - mntnd.

# How to add a project to mntnd?

First of all, you can't just give us a suggestion and leave. Here are our conditions:

* The project must be officially deprecated or it can also be abandoned for more than a year.
* The project must be popular. The meajurement of "popularity" differs from software to software, so we would have to look at each case individually. The projects widely used by big companies are more likely to get accepted.
* **You** must find the project manager - the new maintainer.
* The project manager must accept our [conditions](./manager.md).

Exceptions to the conditions above are possible, but unlikely.

To talk with us about accepting a new project you need to create an issue here: https://github.com/mntnd/.governance

Provide following info:
* the deprecated/abandoned project link,
* proof that it got deprecated/abandoned,
* proof that it is popular,
* proof that the nominated project manager accepts our [conditions](./manager.md).

# What's your governance?

We will try coping the [Apache Software Foundation](https://www.apache.org/theapacheway/index.html) as much as needed but keeping in mind that flexibility and security patches are the top priority.
