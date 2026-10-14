# Castlevania: Bloodlines Password Generator

A password generator for Castlevania: Bloodlines (Sega Genesis / Mega Drive) that runs in any web browser. Pick a character, a difficulty and your version of the game, and it shows the password for every stage.

**Use it online:** https://codekonga.github.io/Castlevania-Bloodlines-Password-Generator/

It's a single HTML file with nothing to install. You can also download `index.html` and open it in any browser, including offline.

## Supported versions

- **US / Europe:** Castlevania: Bloodlines (USA) and Castlevania: The New Generation (Europe), including the Castlevania Anniversary Collection, Mega Drive Mini and Nintendo Switch Online releases. All of these use the same password system.
- **Japan:** Vampire Killer, including the Castlevania Anniversary Collection and Mega Drive Mini releases. Its passwords are laid out differently, so pick the Japan setting for this version.

## Features

- John Morris or Eric Lecarde
- Easy, Normal or Expert (an Expert password also unlocks Expert mode)
- US / Europe: any number of lives (REST 0–9) and continues (0–7), and passwords for the start of all six stages
- Japan: passwords for the start and the mid-stage checkpoint of every stage (1-1, 1-10, 2-1, 2-6, 3-1, 3-8, 4-1, 4-10, 5-1, 5-8, 6-1, 6-4). Vampire Killer passwords don't store lives or continues.
- Three extra starting points in stage 6 (6-6, 6-8 and 6-11) that the game itself never gives out a password for.

## How the password works

The 16 squares hold 32 bits, two bits per square and one byte per row. Inside are the difficulty, character and stage (plus lives and continues in the US / Europe version), protected by two checksums and scrambled with a random key, so every setup has eight valid passwords. This page always shows the same one; all eight work.

The two formats differ in three ways. Vampire Killer numbers the difficulties one lower, doesn't store lives or continues, and keeps a checkpoint partway through each stage, where the US / Europe version restarts the stage from the beginning. A password made for one version will load in the other but with the wrong difficulty, or not at all.

Everything here comes from each version's own password check and password generator, and the generated passwords were tested in the US, European and Japanese games.

The icons are original drawings made to resemble the game's; no game graphics are included.
