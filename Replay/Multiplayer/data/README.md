# data

> still WIP

The value of `type` will dictate the data.

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
    * (int) `frames`: Total of frame played.
    * (object[]) `events`:
      * (int) `frame`: The frame that the action was initiate.
      * (string) `type`: Possible values are [`"keydown"`](/Replay/Multiplayer/data/keydown.md), [`"keyup"`](/Replay/Multiplayer/data/keyup.md), [`"ige"`](/Replay/Multiplayer/data/ige.md), [`"start"`](/Replay/Multiplayer/data/start.md), [`"targets"`](/Replay/Multiplayer/data/targets.md), [`"full"`](/Replay/Multiplayer/data/full.md) and [`"end"`](/Replay/Multiplayer/data/end.md).
