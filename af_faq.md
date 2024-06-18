# AF Decompilation FAQ

## What exactly is Animal Forest?
It's an N64 game that released exclusively in Japan, which was later ported to GameCube and localized as Animal Crossing. Animal Forest is a literal translation of it's Japanese name, Doubutsu no Mori.

There were many different versions released across multiple platforms and regions, each with significant changes:
- Apr. 2001 - Doubutsu no Mori (N64, Japan)
- Dec. 2001 - Doubutsu no Mori + (GameCube port, Japan)
- Sep. 2002 - Animal Crossing (English localization, USA/Canada)
- Jun. 2003 - Doubutsu no Mori e+ (Japanese release with the localization changes from Animal Crossing and new features)
- Oct. 2003 - Animal Crossing (Australian release)
- Sep. 2004 - Animal Crossing (European release)
- Jun. 2006 - Dongwu Senlin (iQue, Chinese localization of Doubutsu no Mori)

## What about the other versions?
This decomp focuses only on the N64 version. However, there is a decomp project for Animal Crossing [here](https://github.com/Prakxo/ac-decomp/).

## I want to help, how can I contribute?
We gladly accept contributions! If you're interested in helping with this project, the first step would be to join our discord server. Project discussion happens in the `#af-decomp` channel.

To work on the project you will need:
- A Linux environment, or WSL through Windows
- Basic knowledge about using command line Git
- Basic knowledge about programming in C. 

Deep programming experience is unnecessary, and you can learn things as needed by working on the project. Experience with MIPS assembly code is also unnecessary, although can be helpful when matching functions. You will not need to write any assembly code in this project.

## Why is this a part of ZeldaRET?
Animal Forest is built off the same codebase as Ocarina of Time and Majora's Mask. We can use the knowledge gained from those projects when decompiling Animal Forest.

## What language was this game written in?
Animal Forest was originally written in C using the C89 standard, which is compiled to MIPS assembly language.

## What compiler was used?
IRIS Development Option (IDO) 7.1

## Can this be used for modding?
In the future, yes! Currently there are some obstacles that limit what can be modified, such as hard coded pointers.

## What is asset analysis?
N64 ROMs have no filesystem and everything is statically linked. This includes assets such as textures, vertices, display lists, and animations, which are all combined into unlabeled blobs of data. In order to extract it into human readable formats, we need to document what this data contains.
