---
title: "How to play"
description: "The rules of Lattice Five (Morpion Solitaire / Join Five), in pictures."
---

Lattice Five is **Morpion Solitaire** (*Join Five*) — a solitaire played on
grid paper since the 1970s. The rules fit in a paragraph; mastering them
doesn't.

## The move

Place one new dot, then draw a straight line through **five dots in a row** —
horizontal, vertical, or either diagonal. The line has to run through the dot
you just placed. Your score is the number of lines you draw.

{{< diagrams >}}
{{< board cols="7" rows="3" dots="0,1 1,1 2,1 3,1" ring="4,1"
   label="Four dots in a row with a fifth position circled" caption="Place a dot…" >}}
{{< board cols="7" rows="3" dots="0,1 1,1 2,1 3,1 4,1" fresh="0,1 1,0 5"
   label="The five dots now joined by a line" caption="…and draw its line" >}}
{{< /diagrams >}}

## The one rule that matters

Two lines running the same direction may **share an end dot**, but they can
never **overlap** — no stretch between two dots is ever drawn twice. Every
line you draw uses up four of those stretches for good, which is why a board
slowly closes in on itself.

{{< diagrams >}}
{{< board cols="11" rows="3" dots="0,1 1,1 2,1 3,1 4,1 5,1 6,1 7,1 8,1"
   line="0,1 1,0 5" fresh="4,1 1,0 5" offset="7"
   label="Two lines meeting at a single shared dot" caption="Allowed — they meet at one dot" >}}
{{< board cols="11" rows="3" dots="0,1 1,1 2,1 3,1 4,1 5,1 6,1 7,1"
   line="0,1 1,0 5" bad="3,1 1,0 5"
   label="A second line overlapping the first" caption="Not allowed — they overlap" >}}
{{< /diagrams >}}

In the stricter **5D** variant, even sharing that one dot is out: lines along
the same direction may not touch at all.

## Five in a row is not a line

A move has to *add* a dot, and the line has to pass through it. Five dots that
were already sitting in a row are worth nothing — and if one placement opens up
two lines at once, you draw one and lose the other.

{{< diagrams >}}
{{< board cols="8" rows="3" dots="0,1 1,1 2,1 3,1 4,1 6,1" bad="0,1 1,0 5"
   label="Five existing dots in a row, marked as not playable" caption="Nothing to claim here" >}}
{{< /diagrams >}}

## Gaps you close off

When two of your lines end up a few dots apart along the same direction,
nothing can ever span the space between them. The app marks those dead gaps
faintly in red, as you play and in replays — a quiet note that some room went
to waste.

{{< diagrams >}}
{{< board cols="13" rows="3" dots="0,1 1,1 2,1 3,1 4,1 7,1 8,1 9,1 10,1 11,1"
   line="0,1 1,0 5" bad="4,1 1,0 4"
   label="Two lines with a dead gap between them" caption="The gap between can never be filled" >}}
{{< /diagrams >}}

## How good is good?

On the classic cross under 5T rules, beginners typically reach the 40s–60s.
The **human record of 170** was set by hand in 1976 and stood for 34 years;
the best computer-found game is **178**. Nobody knows the true maximum —
only that it's at most 485.

## In the app

- **Tap** an empty point to see every line it could make; tap a line to
  play it. Drag over the candidates and lift to choose. Hover works too,
  with a mouse or trackpad.
- **Slide a finger** across the board and it buzzes wherever a dot can go, so
  you can hunt for a move by feel. With a hardware keyboard, arrows or WASD
  roam a cursor and Return places and commits.
- **Free play** offers unlimited undo and all the variants; the **daily**
  is one attempt at the day's shared board, one undo per move.
- The chart under the board shows your position's **openness** — legal
  moves available — against your best game's curve. Stay above the ghost.
- The rules are in the app too: the **?** button on the board.
