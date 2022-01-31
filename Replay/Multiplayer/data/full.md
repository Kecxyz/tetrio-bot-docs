# `"type": "full"`

> ## **WIP**

## Format

* (string) `type`: `"full"`
  * (obj) `data`:
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
    * (object) `options`: Include Room/Hidden/Unmodifiable config, and player handling/customization(?) For room config see [Room_Config](//Room_configmd) For player see `stats`, for some option not listed in Room_Config see below
      * (int) `fulloffset`:
      * (int) `fullinterval`:
      * (unknown?) `onfinish`: null,
      * (unknown?) `oninteraction`: null
      * (string) `username`:
      * (int) `boardwidth`: The width of the board. Default value is 10, seems to be only modifiable server side.
      * (int) `boardheight`: The amount of rows that is visible. Default value is 20, seems to be only modifiable server side.
      * (int) `boardbuffer`: The amount of rows beyond the topout line. Default value is 20, seems to be only modifiable server side.
      * (boolean) `physical`: not sure about this
      * (object) `minoskin`:
        * (string) `z`: `tetrio`
        * (string) `l`: `tetrio`
        * (string) `o`: `tetrio`
        * (string) `s`: `tetrio`
        * (string) `i`: `tetrio`
        * (string) `j`: `tetrio`
        * (string) `t`: `tetrio`
        * (string) `other`: `tetrio`
      * (string) `ghostskin`: `tetrio`
      * (string) `boardskin`: `generic`
    * (object) `stats`:
      * (int) `seed`:
      * (int) `lines`:
      * (int) `level_lines`:
      * (int) `level_lines_needed`:
      * (int) `inputs`:
      * (int) `holds`:
      * (object) `time`:
        * (int) `start`: 0,
        * (boolean) `zero`: true,
        * (boolean) `locked`: false,
        * (int) `prev`: 0,
        * (int) `frameoffset`: 0
      * (int) `score`:
      * (int) `zenlevel`:
      * (int) `zenprogress`:
      * (int) `level`:
      * (int) `combo`:
      * (int) `currentcombopower`:
      * (int) `topcombo`:
      * (int) `btb`:
      * (int) `topbtb`:
      * (int) `tspins`:
      * (int) `piecesplaced`:
      * (object) `clears`:
        * (int) `singles`:
        * (int) `doubles`:
        * (int) `triples`:
        * (int) `quads`:
        * (int) `realtspins`:
        * (int) `minitspins`:
        * (int) `minitspinsingles`:
        * (int) `tspinsingles`:
        * (int) `minitspindoubles`:
        * (int) `tspindoubles`:
        * (int) `tspintriples`:
        * (int) `tspinquads`:
        * (int) `allclear`:
      * (object) `garbage`:
        * (int) `sent`:
        * (int) `received`:
        * (int) `attack`:
        * (int) `cleared`:
      * (int) `kills`:
      * (object) `finesse`:
        * (int) `combo`:
        * (int) `faults`:
        * (int) `perfectpieces`:
    * (string[]) `targets`:
    * (int) `fire`:
    * (object) `game`:
      * (string[]) `board`:
      * (string[]) `bag`:
      * (object) `hold`:
        * (string?) `piece`:
        * (boolean) `locked`:
      * (float?/double?) `g`:
      * (object) `controlling`:
        * (int?/float?) `ldas`:
        * (int?/float?) `ldasiter`:
        * (boolean) `lshift`:
        * (int?/float?) `rdas`:
        * (int?/float?) `rdasiter`:
        * (boolean) `rshift`:
        * (int?/float?) `lastshift`:
        * (boolean) `softdrop`:
      * (object) `handling`:
        * (float) `arr`:
        * (float) `das`:
        * (float) `dcd`:
        * (int) `sdf`:
        * (boolean) `safelock`:
        * (boolean) `cancel`:s
      * (boolean) `playing`:
    * (object) `killer`
      * (string?) `name`:
      * (string) `type`:
    * (object) `assumtions`:
    * (object) `aggregatestats`:
      * (float) `apm`:
      * (float) `pps`:
      * (float) `vsscore`:

TODO: lots of testing required.
