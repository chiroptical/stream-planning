Stream Planning and Goals
---

This repository will contain stream plans and goals for the upcoming month.

### October 2020 (Hacktoberfest)

- [ ] Implement `unison completions`
  - See https://github.com/unisonweb/unison/issues/1670
  - Add `completions` command to https://github.com/unisonweb/unison/blob/df653686004a6fddb89a559ce501371c75d9a099/parser-typechecker/unison/Main.hs#L50
  - Add `completions` pattern match to https://github.com/unisonweb/unison/blob/df653686004a6fddb89a559ce501371c75d9a099/parser-typechecker/unison/Main.hs#L151
  - Add `Completions.hs` to `parser-typechecker/unison` with completions code
  - Example completions available here: https://github.com/kitzeslab/opensoundscape/blob/develop/opensoundscape/completions.py

- [ ] Write "Creating Abilities" Tutorial for Unison
  - See https://www.unisonweb.org/docs/abilities#creating-and-handling-abilities
  - Reorganize the section to connect `emit : e -> ()` with `handle k () with h ...`
    - The `emit` function defines what `k` must input (the return type of `emit`)
    - The `h` function must take the accumlator/s to continue with
  - Add exercises with increasing difficulty
  - Code available `/home/bmooreii/src/unisonweb-org/src/data/docs/abilities.md`

- [ ] **Bonus** Build and release `servant-oauth`
  - Need servant-generic server routes served on `/oauth2`
    - Routes include `/authorize` and `/callback` configured to some OAuth
      provider
  - Need servant-client functions specialized for some OAuth2 provider
  - Need better error handling for client functions
  - Need final style GADT for token storage (in-memory)
