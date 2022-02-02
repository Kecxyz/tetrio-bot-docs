# `"type": "ige"`

**I**n **G**ame **E**vent (IGE) is a type describing interaction between players.

> (Everything described here is assuming that ige only be used for sending information about garbage.)

## Formats

* (string) `type`: `"ige"`
  * (obj) `data`:
    * (int) `id`: Increment from 0 for each `"ige"` type.
    * (string) `type`: `"ige"`
    * (object) `data`:
      * (string) `type`: `"interaction"` for the frame you receive the information about garbage. `"interaction_confirm"` for the frame that you actually receive garbage.
      * (object) `data`:
        * (string) `type`: only possible value is `"garbage"`(? not sure)
        * (int) `amt`: Amount of garbage that was received.
        * (int) `x`: Horizontal position of the piece that cleared the line that sent you the garbage.
        * (int) `y`: Vertical position of the piece that cleared the line that sent you the garbage.
        * (int) `column`: Which column garbage will appear in on your board.
      * (string) `sender`: Username of who sent the garbage.
      * (int) `sent_frame`: Which frame the garbage was sent on.
      * (int) `cid`: Increment for each pair of `"interaction"` and `"interaction_confirm"`.

TODO: more testing.
