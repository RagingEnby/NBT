# NBT

This directory restores the Python source from RagingEnby's NBT fork. The source came from the installed NBT 1.5.1 package in Skypixel's virtual environment. Its installation metadata records commit `7c672e11c4daaef3c1ee070c2e401e4b7b9efff8` from `https://github.com/RagingEnby/NBT`.

All five recovered Python files are unchanged. `recovery.json` records their SHA-256 hashes. The MIT license is included in `LICENSE.txt`. This copy retains the fork's `mutf8` dependency.

The installed package did not contain Git history, so this fork starts from upstream `twoolie/NBT` and applies the recovered files in one commit. The upstream tests, examples, docs, and `setup.py` remain. `pyproject.toml` and this README were written during recovery.

Use Python 3.11 or later. Install this copy with `python -m pip install .` or `uv pip install .`.

```python
from nbt import nbt

data = nbt.NBTFile("example.nbt")
print(data.pretty_tree())
```
