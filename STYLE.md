# Our coding style

Rules we agreed on so the code looks the same whoever wrote it. The examples
come from our own hello.py, hello.js and hello.c.

- **Names say what they hold.** `word` in hello.py, not `w` or `x`. If the name
  is vague I have to read the next few lines to work out what is inside it,
  which is wasted time every single time.

- **Indent consistently.** Python forces you to. C does not, so it is easy to
  let it slide. In hello.c everything inside main() is indented four spaces and
  the loop body goes one level deeper than that.

- **Comment the why, not the what.** `i--; // decrease i` just repeats the code.
  The useful comment in hello.c is the one saying the loop runs backwards on
  purpose, because that is not obvious from looking at it.

- **Keep lines short.** Around 80 characters. This is the rule I break most
  often, usually when I add a note to myself at the end of a line.

- **Leave a blank line between steps.** hello.c reads as three parts: the
  includes, the setup, then the printing. The blank lines are what let you see
  those parts without reading closely.

- **Clear beats clever.** `word[::-1]` is clever and short, but
  `"".join(reversed(word))` says out loud what it is doing. In hello.py I used
  the short one because the file is three lines long. In a real program I would
  write it out.

- **Every project has a README.** It should say what the project is and how to
  run it, so someone who has never seen the folder can get it going without
  asking me.
