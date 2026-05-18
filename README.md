# Chromium Compatible Mongolian Spellcheck Dictionary

This repository contains a Chromium-compatible version of the Mongolian spellcheck dictionary, natively optimized for browsers such as Google Chrome, Brave, and Microsoft Edge.

The core data is based on the official orthographic dictionary of Ts. Damdinsuren (1983).

## Architecture & The Flattening Process

Standard Hunspell dictionaries utilize continuation classes to chain suffixes and save memory. However, Chromium's binary dictionary compiler (`convert_dict`) fails to accurately parse multi-level chained rules, leading to broken spellcheck behavior.

**Upstream core data repository:** [https://github.com/bataak/dict-mn](https://github.com/bataak/dict-mn)
