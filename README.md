# smart-text-randomizer <sup>v0.1.0</sup>

Smart Text Randomizer

---

[![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smart-text-randomizer)](https://github.com/smartlegionlab/smart-text-randomizer/)
![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/smart-text-randomizer)
[![GitHub](https://img.shields.io/github/license/smartlegionlab/smart-text-randomizer)](https://github.com/smartlegionlab/smart-text-randomizer/blob/master/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/smartlegionlab/smart-text-randomizer?style=social)](https://github.com/smartlegionlab/smart-text-randomizer/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/smartlegionlab/smart-text-randomizer?style=social)](https://github.com/smartlegionlab/smart-text-randomizer/network/members)
[![PyPI Downloads](https://static.pepy.tech/badge/smart-text-randomizer)](https://pepy.tech/projects/smart-text-randomizer)
[![PyPI - Downloads](https://img.shields.io/pypi/dm/smart-text-randomizer?label=pypi%20downloads)](https://pypi.org/project/smart-text-randomizer/)
[![PyPI](https://img.shields.io/pypi/v/smart-text-randomizer)](https://pypi.org/project/smart-text-randomizer)
[![PyPI - Format](https://img.shields.io/pypi/format/smart-text-randomizer)](https://pypi.org/project/smart-text-randomizer)

---

## ⚠️ Disclaimer

**By using this software, you agree to the full disclaimer terms.**

**Summary:** Software provided "AS IS" without warranty. You assume all risks.

**Full legal disclaimer:** See [DISCLAIMER.md](https://github.com/smartlegionlab/smart-text-randomizer/blob/master/DISCLAIMER.md)

---

## Help:

`pip install smart-text-randomizer`

"Text randomization" or "variable text". It is used to create different variations of the same message.

You are using special syntax. Example: `'{Salute|Hello|Good morning} {comrade|buddy|dear friend}!'`

This syntax allows you to create variable messages by using curly braces and vertical bars to indicate alternatives.

Basic elements of syntax:

1. Curly braces {}: Used to group text options. Anything inside the curly braces will be randomly selected when generating the text.
2. Vertical bar |: Used to separate different text options within curly braces. Each option will be treated as a separate choice.

Example of use:

- Syntax: `'{Salute|Hello|Good morning} {comrade|buddy|dear friend}!'`
- Possible results:
    - Salute comrade!
    - Salute buddy!
    - Salute dear friend!
    - Hello comrade!
    - Hello buddy!
    - Hello dear friend!
    - Good morning comrade!
    - Good morning buddy!
    - Good morning dear friend!
- How to use:
  1. Create your text: Identify which parts of your message can vary and place them in curly braces.
  2. Add options: Separate alternatives with a vertical bar.
  3. Text Generation: Use RandomStringMaster() to generate a random message.

- Notes:
    - Make sure all options inside the curly braces make sense and fit the context.
    - You can use multiple randomization groups in a single message to create more complex variations.


Example of text randomization:

```python
from smart_text_randomizer import TextRandomizer

text_randomizer = TextRandomizer()

text = '{Salute|Hello|Good morning} {comrade|buddy|dear friend}!'
randomized_text = TextRandomizer.randomize(text)
print(randomized_text) # Good morning buddy!
```

---

## License

**[BSD 3-Clause License](https://github.com/smartlegionlab/smart-text-randomizer/blob/master/LICENSE)**

Copyright (©) 2026, [Alexander Suvorov](https://github.com/smartlegionlab)

---
