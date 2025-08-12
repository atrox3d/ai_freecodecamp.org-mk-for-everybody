# ML for everyone
[video of the course](https://youtu.be/i_LwzRVP7bg?si=FvVAVs8tJDKZs_qi)

# datasets

## Magic Gamma Telescope Data Set
[magic gamma telescope dataset](https://archive.ics.uci.edu/dataset/159/magic+gamma+telescope)

## Seoul Bike Sharing Demand Data Set
[seoul bike sharing demand dataset](https://archive.ics.uci.edu/dataset/560/seoul+bike+sharing+demand)

---

# troubleshooting

## tensorflow

I ran into an issue where I could not install `tensorflow` via `uv` with Python 3.12. After pinning the version to 3.10, I still could not import the library.

### Solution

The following steps resolved the installation issue:

1.  **Pin Python to version 3.10:**
```bash
uv python pin 3.10      # set uv venv python version to 3.10
# modified .python.version file
# modified pyproject.toml file (requires-python = ">=3.10")

rm -rf .venv            # remove old env just to be sure
uv sync                 # recreate venv

uv python find          # check that the current uv python is the correct one
uv run python -V        # check the version
```

2. **install tensorflow via pip**

```bash
uv pip install tensorflow
```


not sure if it's the correct way, but i just needed to finish the course and it worked

- Added a pip freeze output to pip-requirements.txt, just in case