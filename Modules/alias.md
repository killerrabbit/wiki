---
title: Modules &raquo; m_alias
layout: default
---

## Description

This module allows aliases to be made for commands. Aliases can be quite
complex and can shorten commands or act as fantasy commands.

### Configuration Tags

`<alias text="Command" replace="text to replace command with" usercommand="true" channelcommand="false" format="#aglob*pattern" requires="nick" uline="true" operonly="false">`

Setting | Description
------- | -----------
text="Command" | Command to trigger alias
replace="text to replace command with" | Text to replace command with
usercommand="true" | Allows command to be with /alias
channelcommand="false" | Allows command to be used in a channel with fantasy prefix
format="#aglob*pattern" | Parameters must match this glob for alias to trigger
requires="nick" | Requires nick to be online on the network to trigger
uline="true" | Requires nick to be on a ulined server
operonly="false" | Only allows ircops to trigger alias

`<fantasy prefix="!" allowbots="no">`

Setting | Description
------- | -----------
prefix="!" | Prefix used for aliases inside of channels
allowbots="no" | Ignore alias triggers from "bot" users(m_botmode)

## Modes

This module does not implement any extra user or channel modes.

## Extended Bans

This module implements no extended bans.

## Commands

None, but allows existing commands to be aliased.

## Special Notes

This module is commonly used to alias commands such /nickserv to /msg nickserv.
`<alias text="NICKSERV" replace="PRIVMSG NickServ :$2-" requires="NickServ" uline="yes">`
