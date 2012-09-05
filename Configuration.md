---
title: Configuration 
layout: default
---

## Introduction

Configuring InspIRCd -as any other ircd- is not an easy task. Since InspIRCd is as featurefull as it
is, there is a lot to configure. But, not to panic, there is this documentation! Configuration of
InspIRCd is done by editing the configuration text file, usually called inspircd.conf. The
inspircd.conf file is formatted as a XML-alike document, which for most people is somewhat different
to what they are used to. The format of an instruction within the configuration file looks like the
following:
    <tagname variable="value">

There may be one or more variables in the tag, each of which must have exactly one value. A variable
must be followed immediately by an equals sign and then its value in quotes, with no spaces between
the two, as shown in this example. The tagname must contain only alphabetical characters. 

You **do not** require closing tags as in XML.

We provide example config files with each InspIRCd release, which are automatically copied in the
config dir. These examples are the best configuration-documentation there is, so use them to your
advantage! Since these examples cover most of the things that InspIRCd features, we will give only
additional information on this wiki.

## Isn't there an easier way?

We try to make installing and configuring as easy as possible. However, configuring an ircd is not a
simple task, especially when an ircd is as powerfull as InspIRCd. Many defaults in the example
configfiles will work perfectly to begin your ircd with. When you get to the advanced stuff, you can
check on the wiki or ask anything in our support channel.
