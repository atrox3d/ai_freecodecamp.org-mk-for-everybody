# ML for everyone
[video](https://youtu.be/i_LwzRVP7bg?si=FvVAVs8tJDKZs_qi)

# Magic Gamma Telescope Data Set
[dataset](https://archive.ics.uci.edu/dataset/159/magic+gamma+telescope)


# troubleshooting

## tensorflow

        could not install tensorflow via uv with python 3.12

        after pinning python to 3.10 and adding tensorflow could not import it



- had to pin python version to 3.10

```bash
uv python pin 3.10
```

- had to install tensorflow via pip

```bash
uv pip install tensorflow
```


not sure if it's the correct way, but i just need to finish the course
