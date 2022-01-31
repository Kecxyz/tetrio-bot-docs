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
    * (int) `frames`:
    * (object[]) `events`:
      * (int) `frame`:
      * (string) `type`: Possible values are `"keydown"`, `"keyup"`, `"ige"`, `"start"`, `"targets"`, `"full"` and `"end"`.
