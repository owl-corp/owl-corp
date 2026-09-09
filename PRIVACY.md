# Privacy Policy

*Last updated: 9th September 2026*

This document details what data Owl Corp stores on you as a user of Polonium,
our modmail bot. Privacy and security of user data is one of our top
priorities while running Polonium. This document sets out what data we store, why
we need it, who has access to it, and how we process it. Please see the
[terminology](#terminology) section to better understand this document.

This document is inspired by the [Python Discord Privacy Policy](https://pythondiscord.notion.site/Privacy-Policy-4ceb50b84d164541bd5b0b7046aa7e6a).

## Table of contents

- [What data do we store?](#what-data-do-we-store)
- [What data do we not store?](#what-data-do-we-not-store)
- [Assurance on processing](#assurance-on-processing)
- [Services](#services)
  - [Bot](#bot)
  - [API and Database](#api-and-database)
  - [Sentry](#sentry)
- [Contact](#contact)
- [Terminology](#terminology)

## What data do we store?

We store message contents and Discord IDs tied to modmail conversations. This is
essential to Polonium's operation, since a moderator needs to be able to read and
reply to what a user sent, and to look back over a post's history later.

When a user opens or is added to a modmail post, we store their Discord user ID and
the guild roles used to determine permission levels of staff replying to posts.

## What data do we not store?

We do not knowingly store the data of users under 13. On becoming aware of a user
who is below the age of 13 we forward this information on to Discord, who take
action on the user as they find appropriate. Once this user has been deleted from
Discord we remove data we hold on them.

We do not store message contents from anywhere other than modmail conversations
sent to or from Polonium.

## Assurance on processing

We take numerous steps to ensure data is handled carefully. Direct database access
is only available to the developers who run Polonium.

Modmail post contents are only accessible to server moderators, and only through
Polonium's own commands (such as `/logs` and `/history`).

We ensure that all data we store is critical to operation and do not store more
than is needed. We aim to be as transparent as possible on what data we store and
for what purpose.

## Services

Below is service specific information of what data we hold. There is an entry for
every service we run which stores user data, and any third-party service which has
access to some user data.

### Bot

<details>
<summary>User IDs</summary>

Internal structures in the bot use user IDs to look up the guild member a DM
belongs to, and to check the permission level of whoever is replying to a post.

</details>

<details>
<summary>User–Bot DMs</summary>

Modmail conversations happen through DMs with the bot. Message content sent in
these DMs is relayed into the corresponding modmail post, and is not stored by
the bot itself beyond what's needed to forward it.

</details>

### API and Database

<details>
<summary>Discord user IDs</summary>

Used to tie modmail posts, messages, and permission levels to a specific user,
so moderators can find a user's post history even after they leave the post.

</details>

<details>
<summary>Guild and role configuration</summary>

Stores which forum channel modmail posts are created in, and which roles are
permitted to reply to posts, so the bot knows where to route messages and who
is allowed to act on them.

</details>

<details>
<summary>Modmail post and thread metadata</summary>

Stores whether a post is open or closed and its reminder status, so we can
notify moderators if a post goes unanswered for too long.

</details>

<details>
<summary>Message contents</summary>

Message contents sent through modmail posts are stored so moderators can search
and review conversation history using `/logs` and `/history`.

</details>

### Sentry

We use [Sentry](https://sentry.io/) for managing errors within our services.

<details>
<summary>Discord user IDs and usernames</summary>

May appear in an error's context (e.g. which user or command triggered it) when
an error is reported.

</details>

## Contact

Any questions regarding this privacy policy can be addressed to the Owl Corp Data
Controller via email to ops@owlcorp.uk, or through our
[support server](https://discord.gg/k82eWxBkQC).

We can erase certain data items upon request, please contact us through one of the
above methods and we will do our best to fulfil it.

## Terminology

| Term                          | Also referred to as    |
|--------------------------------|-------------------------|
| Owl Corp                       | we, our, us             |
| The Discord server Polonium runs in | guild, server, community |
| A user of Polonium              | user, you, your          |
