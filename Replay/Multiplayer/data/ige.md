# `"type": "ige"`

**I**n **G**ame **E**vent (ige) is an event describing interaction between players.

## Formats

* (string) `type`: `"ige"`
  * (obj) `data`:
    * (int) `id`: Enumerate from 0 for each `"ige"` type.
    * (string) `type`: `"ige"`
    * (object) `data`:
      * (string) `type`: `"interaction"` for the frame you receive the information about garbage. `"interaction_confirm"` for the frame that you actually receive garbage.
      * (object) `data`:
        * (string) `type`: only possible value is `"garbage"`(? not sure)
        * (int) `amt`: Amount of garbage that was sent.
        * (int) `x`: Horizontal position of the piece that cleared the line that sent garbage.
        * (int) `y`: Vertical position of the piece that cleared the line that sent garbage.
        * (int) `column`: Which column garbage will appear in.
      * (string) `sender`: Username of who sent the garbage.
      * (int) `sent_frame`: Which frame the garbage was sent on.
      * (int) `cid`: Enumerate for each pair of `"interaction"` and `"interaction_confirm"`.

TODO: more testing.
