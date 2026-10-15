# gadgets-games-tetris

Tetris for the gadgets of [polpo](https://github.com/polpo-system/polpo): fit the falling pieces into full rows.

```
portia.Install gadgets-games-tetris
```

## Playing

    Desktops.OpenDoc Tetris.Panel       the panel: levels, backdrops, Start Tetris, New High
    Desktops.OpenDoc (Tetris.NewDoc)    a game without the panel

The keys are listed on the panel (the arrow keys move, rotate and drop).

`tools/Tetris.Tool` has these commands to click.

## What is here

    src/Tetris.Mod             the game
    share/Tetris.Panel         the panel
    share/Bows.Pict, Bricks.Pict, Cells.Pict, Clouds.Pict, Coins.Pict, Fractal.Pict,
          Molecules.Pict, Spirals.Pict, Surface.Pict, Textils.Pict    the backdrops of the levels
    tools/Tetris.Tool
    test/TetrisTest.Mod

Tetris is by Wolfgang Ibl (after Alexey Pajitnov and Vadim Gerasimov), from ETH Native Oberon
2.3.6. The source was converted from an Oberon text to plain text; the first commit has it
unchanged. It compiles unchanged with all five of polpo's compilers (x86, ARM, ARMv7, RISC-V,
MIPS). The icon of its documents comes from gadgets-icons3.

## Tests

    TetrisTest.Run      2 checks: a game document made and loaded; it needs the desktop's display

The license is GPL-3 (`LICENSE`); the code comes from ETH Oberon, whose license (`LICENSE.ETH`)
asks to keep its copyright notice and conditions, which `LICENSE.ETH` does.
