+++
title = "Writing a BitBoard in Rust Pt. 2: The Game State"
date = "2021-09-14T08:11:54+02:00"
author = ""
authorTwitter = "" #do not include @
cover = ""
draft = true
tags = ["rust", "chess", "bitboard"]
keywords = ["rust", "chess", "bitboard"]
description = "Now that we have a bitboard to store the pieces, we need a way to store the game state"
showFullContent = false
+++

## Explanation

The state will contain only the necessary information to evaluate a position outside the pieces positions.
So it contains the:
- Castling rights 
- Half move counter
- Side to move
- En passant(if possible)

