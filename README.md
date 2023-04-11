# pdm-manage-version

Wanted something like `poetry version` in `pdm`.

Add the plugin using:

```shell
pdm plugin add pdm-manage-version
```

## Alternatives

I found [https://github.com/abersheeran/pdm-version/](https://github.com/abersheeran/pdm-version/) but
it doesn't really behave like `poetry version` unfortunately

## How to use

### `pdm version`

It will print the current version, it will only output the version

```shell
$ pdm version
0.1.0
```

### `pdm version <next-version>`

Bumps/changes the version in pyproject. `<next-version>` can either be one of `major`, `minor`, `patch` or `micro` or the next version you want:

```shell
$ pdm version
0.1.0
$ pdm version major
1.0.0
$ pdm version minor
1.1.0
$ pdm version patch
1.1.1
$ pdm version micro
1.1.2
$ pdm version minor
1.2.0
$ pdm version 5.0.0
5.0.0
```

## ToDo:

- [ ] Tests
- [ ] Better bump logic
