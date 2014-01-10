---
title: Modules &raquo; m_auditorium
layout: default
---

## Description	

Provides a channel mode to hide joins/parts/quits in a channel.

## Configuration Tags

`<auditorium opvisible="no" # Are channel ops visible to all in the channel?
opcansee="no" # Can channel ops see every user in the channel?
opercansee="yes">` # Can ircops see all in the channel?

## Commands

This module does not implement any commands.

## User Modes

This module does not implement any user modes.

## Channel Modes

Mode | Description
---- | -----------
u | Set this mode to turn on auditorium mode and hide joins/parts/quits.

Example: `/mode #channel +u`

## Extended Bans

This module does not implement any extended bans.
