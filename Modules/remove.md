---
title: Modules &raquo; m_remove
layout: default
---

## Description	

Provides a `/remove` command, this is mostly an alternative to
`/kick`, except makes users appear to have parted the channel

## Configuration Tags

`<remove supportnokicks="yes">`

## Commands

`/REMOVE <nick> <channel> [message]`

Forceparts the user from the channel, requires halfops or higher.

`/FPART <channel> <nick> [message]`

This behaves identically to `/REMOVE`, the only difference is that
that `<channel>` and `<nick>` parameters are switched around to match
`/KICK`'s syntax. Also, `/REMOVE` is a builtin mIRC command which
caused trouble for some users. This feature was added in the 1.1
branch.

## User Modes

This module does not implement any user modes.

## Channel Modes

This module does not implement any channel modes.

## Extended Bans

This module does not implement any extended bans.

## Notes

When `+haq` are enabled, then you may forcepart anyone with a equal or
lower 'level' than you, and if you are `+a` or `+q` you do not require
`+o` to use `/REMOVE`.

For example:

* UserA has modes +o
* UserB has modes +oa (effectively +a)
* UserC has modes +v
* UserD has modes +q

In this example:

* UserA can only forcepart UserC as they are the only user with the same or lower level.
* UserB can forcepart UserA and UserC, UserB's +o is ignored, as +a is 'higher' than it.
* UserC can forcepart nobody, you must be at least a halfop to forcepart a user.
* UserD can forcepart anyone on the channel, even though he doesn't have ops. 

## Extra Resources

