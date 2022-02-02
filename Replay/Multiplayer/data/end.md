# `"type": "end"`

> Anything listed here are subject to change at any moment

State of the round when the round end. This include room settings, player handling, line cleared, board state, player stats, etc.  

## Format

* (string) `type`: `"end"`
  * (obj) `data`:
    * (string) `reason`:
      * (boolean) `successful`: Seems to be solo only value?
      * (string?) `gameoverreason`: Null at frame 0/or if the player won Possible value are `topout` or `garbagesmash`
      * (object) `replay`:
        * (unknown?) `advanceFrame`: Seems to be null only?
        * (unknown?) `getFrame`: Seems to be null only?
        * (unknown?) `getEventCount`: Seems to be null only?
        * (unknown?) `getStarter`: Seems to be null only?
        * (unknown?) `getStartEvent`: Seems to be null only?
        * (unknown?) `getEndEvent`: Seems to be null only?
        * (unknown?) `pushEvent`: Seems to be null only?
        * (unknown?) `getEventsAtFrame`: Seems to be null only?
        * (unknown?) `export`: Seems to be null only?
        * (unknown?) `import`: Seems to be null only?
        * (unknown?) `seek`: Seems to be null only?
        * (unknown?) `bindRolling`: Seems to be null only?
        * (unknown?) `setListenID`: Seems to be null only?
        * (unknown?) `flush`: Seems to be null only?
        * (unknown?) `amendTargets`: Seems to be null only?
        * (unknown?) `setLatencyPreference`: Seems to be null only?
      * (object) `source`:
        * (unknown?) `advanceFrame`: Seems to be null only?
        * (unknown?) `getFrame`: Seems to be null only?
        * (unknown?) `readyEventQueue`: Seems to be null only?
        * (unknown?) `pull`: Seems to be null only?
        * (unknown?) `nextFrameReady`: Seems to be null only?
        * (unknown?) `fallingBehind`: Seems to be null only?
        * (unknown?) `amountToCatchUp`: Seems to be null only?
        * (unknown?) `behindness`: Seems to be null only?
        * (unknown?) `bind`: Seems to be null only?
        * (unknown?) `unbind`: Seems to be null only?
        * (unknown?) `seek`: Seems to be null only?
        * (unknown?) `finished`: Seems to be null only?
        * (unknown?) `type`: Seems to be null only?
        * (unknown?) `pushIGE`: Seems to be null only?
        * (unknown?) `pushTargets`: Seems to be null only?
        * (unknown?) `unhook`: Seems to be null only?
        * (unknown?) `destroy`: Seems to be null only?
        * (unknown?) `socket`: Seems to be null only?
        * (unknown?) `bindHyperRetry`: Seems to be null only?
        * (unknown?) `bindHyperForfeit`: Seems to be null only?
      * (object) `options`: Include Room/Hidden/Unmodifiable config, and player handling/customization(?) For room config see [Room_Config](../../../Room_Config.md) For player see `stats`, for some option not listed in Room_Config see below
        * (int) `fulloffset`: Unknown
        * (int) `fullinterval`: Unknown
        * (unknown?) `onfinish`: Unknown, seems to be null only?
        * (unknown?) `oninteraction`: Unknown, seems to be null only?
        * (string) `username`: Player username.
        * (int) `boardwidth`: The width of the board. Default value is 10, seems to be only modifiable server side.
        * (int) `boardheight`: The amount of rows that is visible. Default value is 20, seems to be only modifiable server side.
        * (int) `boardbuffer`: The amount of rows beyond the topout line. Default value is 20, seems to be only modifiable server side.
        * (boolean) `physical`: not sure about this
        * (object) `minoskin`: Player's blockskin. Default is [`"tetrio"`](https://tetr.io/res/skins/minos/tetrio.png). **TODO: connected format test.**
          * (string) `z`: Z piece.
          * (string) `l`: L piece.
          * (string) `o`: O piece
          * (string) `s`: S piece
          * (string) `i`: I piece
          * (string) `j`: J piece
          * (string) `t`: T piece
          * (string) `other`: Garbage hole and already hold. Default is [`"tetrio"`](https://tetr.io/res/skins/minos/tetrio.png). **TODO: connected format test.**
        * (string) `ghostskin`: Ghost piece. Default is [`"tetrio"`](https://tetr.io/res/skins/ghost/tetrio.png). **TODO: connected format test.**
        * (string) `boardskin`: Other board asset such as [queue/hold](https://tetr.io/res/skins/board/generic/queue.png), [grid](https://tetr.io/res/skins/board/generic/grid.png), and [board](https://tetr.io/res/skins/board/generic/board.png)
      * (object) `stats`:
        * (int) `seed`: Queue seed, see [Piece_RNG.md](../../../Piece_RNG.md).
        * (int) `lines`: line cleared.
        * (int) `level_lines`: Unimportant value since there are no leveling in multiplayer default is `0`.
        * (int) `level_lines_needed`: Unimportant value since there are no leveling in multiplayer default is `1`.
        * (int) `inputs`: Number of inputs that has been pressed.
        * (int) `holds`: Number of hold used.
        * (object) `time`:
          * (int) `start`: 0,
          * (boolean) `zero`: true,
          * (boolean) `locked`: false,
          * (int) `prev`: 0,
          * (int) `frameoffset`: 0
        * (int) `score`: Player's score.
        * (int) `zenlevel`: Unimportant value. Default is `1`
        * (int) `zenprogress`: Unimportant value. Default is `0`
        * (int) `level`: Unimportant value since you can't level up in multiplayer. Default is `1`
        * (int) `combo`: Current combo when the round end.
        * (int) `currentcombopower`: Possibly about multiplier? TODO: NEED TESTING
        * (int) `topcombo`: Highest combo.
        * (int) `btb`: Current back to back when the round end.
        * (int) `topbtb`: Highest back to back value.
        * (int) `tspins`: Number of spin cleared.
        * (int) `piecesplaced`: Total piece placed by the player.
        * (object) `clears`:
          * (int) `singles`: Total single clear.
          * (int) `doubles`: Total double cleared
          * (int) `triples`: Total triple cleared
          * (int) `quads`: Total quad cleared
          * (int) `realtspins`: TODO:NEED TESTING
          * (int) `minitspins`: TODO:NEED TESTING
          * (int) `minitspinsingles`: Number of cleared mini single spin.
          * (int) `tspinsingles`: Number of cleared single spin.
          * (int) `minitspindoubles`: Number of cleared mini double spin.
          * (int) `tspindoubles`: Number of cleared double spin.
          * (int) `tspintriples`: Number of cleared triple spin.
          * (int) `tspinquads`: Number of cleared quad spin.
          * (int) `allclear`: Total allclear cleared
        * (object) `garbage`:
          * (int) `sent`: Garbage sent.
          * (int) `received`: Garbage received.
          * (int) `attack`: TODO: Extra testing
          * (int) `cleared`: TODO: Extra testing
        * (int) `kills`:
        * (object) `finesse`:
          * (int) `combo`: im guessing number of pieces with perfect finesse consecutive to each other right be fore the round end. TODO: testing
          * (int) `faults`: Number of finesse fault.
          * (int) `perfectpieces`: Number of piece with perfect finesse.
      * (string[]) `targets`: userid of the player(s) that being send garbage to.
      * (int) `fire`: is the player on fire? TODO : test this
      * (object) `game`:
        * (string[]) `board`: Matrix constructed with `boardheight`+`boardbuffer` as height and `boardwidth` as width, displaying the board final state.
  `null` for empty space,  `"l"` for L piece colored block. `"j"` for J piece colored block. `"o"` for O piece colored block. `"i"` for I piece colored block. `"s"` for S piece colored block. `"z"` for Z piece colored block. `"l"` for L piece colored block. `"gb"` for garbage block.
        * (string[]) `bag`: Current piece in preview with piece the first place as playing piece.
        * (object) `hold`:
          * (string?) `piece`: Current piece in hold.
          * (boolean) `locked`: To see if the hold piece holdable.
        * (float) `g`: gravity value when the round end
        * (object) `controlling`: TODO:all of this need testing.
          * (float?) `ldas`:
          * (float?) `ldasiter`:
          * (boolean) `lshift`:
          * (float?) `rdas`:
          * (float?) `rdasiter`:
          * (boolean) `rshift`:
          * (float?) `lastshift`:
          * (boolean) `softdrop`:
        * (object) `handling`:
          * (float) `arr`: Player's ARR value.
          * (float) `das`: Player's DAS value.
          * (float) `dcd`: Player's DCD value.
          * (int) `sdf`: Player's SDF value.
          * (boolean) `safelock`: Is prevent accidental harddrop on or off.
          * (boolean) `cancel`: Is cancel DAS when changing direction on or off.
        * (boolean) `playing`: True for winner of the round. False for loser.
      * (object) `killer`: Should be who killed the user but there are still name value even when the user won the round? TODO: more testing
        * (string?) `name`:
        * (string) `type`:
      * (object) `assumtions`: Unknown what the do.
      * (object) `aggregatestats`:
        * (float) `apm`: Player's APM stat.
        * (float) `pps`: Player's PPS stat.
        * (float) `vsscore`: Player's VS score.

TODO: lots of testing required.
