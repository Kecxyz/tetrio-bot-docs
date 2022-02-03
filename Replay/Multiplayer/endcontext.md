# endcontext

> **WIP**: this is still a work in progress

Summarization of stats. Which will be recalculate when import replay but useful if you just want quick statistic.

## Format

* (object[]) `endcontext`:
  * (int) `naturalorder`: 1 for winner and 0 for loser.
  * (object) `user`:
    * (string) `id`: Player userid.
    * (string) `username`: Player username.
  * (boolean) `active`: Only false if player disconnected.
  * (int) `wins`: Number of round won.
  * (object) `points`:
    * (int) `primary`: Number of round won.
    * (float) `secondary`: Average APM.
    * (float) `tertiary`: Average PPS.
    * (object) `extra`:
      * (float) `vs`: Average VS score.
    * (float[]) `secondaryAvgTracking`: List of average APM per round.
    * (float[]) `tertiaryAvgTracking`: List of average PPS per round.
    * (object) `extraAvgTracking`:
      * (float[]) `aggregatestats___vsscore`: List of average VS score per round.
  * (int) `inputs`: Total input used.
  * (int) `piecesplaced`: Total piece placed.

TODO: description.
