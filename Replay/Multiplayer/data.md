# > **WIP** this is still a work in progress

## data

## Format

* (object[]) `data`:
  * (object[]) `board`:
    * (object) `user`:
      * (string) `_id`:
      * (string) `username`:
    * (boolean) `active`:
    * (boolean) `success`:
    * (int) `winning`:
  * (object[]) `replays`:
    * (int) `frames`:
    * (object[]) `events`:
      * (int) `frame`:
      * (string) `type`:
      * (obj) `data`:
        * (boolean) `successful`: Seems to be solo only value.
        * (string?) `gameoverreason`: Null at frame 0/or if the player won. Possible value are `topout` or `garbagesmash`.
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
        * (object) `options`: Include Room/Hidden/Unmodifiable config, and player handling/customization(?). For room config see [Room_Config](../../Room_config.md). For player see below.
        * (object) `stats`:
          *
