# tracker

Organization wide memory for Keel Linux, in the shape TurnKey Linux uses: the
issues that do not belong to a single repository live here, and the ones that
do live with their code.

## What goes where

| Where | What |
|-------|------|
| `Keel-Linux/tracker` issues | anything crossing repositories, anything not yet assigned to one, decisions waiting on the maintainer, and the order of work |
| each repository's issues | work whose whole diff lands in that repository |
| `Keel-Linux/handbook` (private) | the running log, the decision notes, and anything naming a host, an address or a credential path |

An issue here says what has to be true when it is closed, and names the
repositories it touches. When the work becomes one diff in one place, it moves
to that repository and this issue closes with a link.

## Why this exists

Decision 0006 of the handbook said the project would have no global tracker,
unlike TurnKey Linux. The maintainer reversed that on 2026-09-27: without one,
cross repository knowledge lives in long documents that have to be read whole,
or in an agent's memory, which is worse. An issue is atomic, it can be closed,
and anybody can read one without reading the rest.

## Conventions

- One issue, one outcome. The title says the outcome, not the activity.
- The body states what is true today, what must be true when it closes, and
  what it depends on.
- Nothing here names a credential, a passphrase or a private address. Those
  belong in the handbook.
