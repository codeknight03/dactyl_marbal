# Dactyl Manuform keymap

This keymap keeps QWERTY stable while training the layers needed for a future
keyboard without a number row.

## Layer rule

- Hold the right-side `LOWER` key to type numbers with the left hand.
- Hold the left-side `RAISE` key to type symbols with the right hand.
- Hold both to enter `ADJUST` for Bluetooth configuration.

The opposite-hand arrangement prevents the layer key from competing with the
fingers doing the useful work.

## NumNav (`LOWER`)

```text
left hand                              right hand

7  8  9  /  *                         Home  Up    End    PgUp
4  5  6  -  +                         Left  Down  Right  PgDn
1  2  3  .  =
            thumb 0
```

The digits follow conventional numpad geometry. The same layer exposes
`F1`–`F12` on the physical top row, including the keys used by Neovim DAP.

## Symbol (`RAISE`)

The right hand contains the symbols most useful for Go, Neovim, tmux, and the
shell:

```text
{  (  )  [  ]  }
!  =  :  "  <  >
-  +  /  *  &  |
```

Design landmarks:

- Parentheses and square brackets are adjacent.
- Braces wrap the delimiter row; opening brace is on the strong inner column,
  while Neovim's `[` and `]` stay adjacent.
- `:=` is an inward roll from `:` to `=`.
- `!=` is an adjacent roll.
- Double quote is on the home row for Go strings.
- Arithmetic and shell operators occupy one row.

The left half holds the less frequent symbols and familiar shifted-number
anchors. Base-layer punctuation remains available during the transition.

## Transition expectations

The base layer is unchanged, so prose, QWERTY commands, Space-leader mappings,
and tmux commands continue to work normally. For two weeks, deliberately use
NumNav for every digit and Symbol for `()`, `[]`, `{}`, `:=`, `!=`, quotes, and
operators. Keep the physical number row as a fallback until layer use is
automatic; removing it before then would make it harder to distinguish a bad
placement from ordinary learning friction.
