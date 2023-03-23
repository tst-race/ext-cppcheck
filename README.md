# Cppcheck for RACE

This repo provides scripts to custom-build the
[Cppcheck tool](https://github.com/danmar/cppcheck) for RACE.

## License

The Cppcheck tool is licensed under the GPL 3.0 license.

Only the build scripts in this repo are licensed under Apache 2.0.

## Dependencies

Cppcheck has no dependencies on any custom-built libraries.

## How To Build

The [ext-builder](https://github.com/tst-race/ext-builder) image is used to
build Cppcheck.

```
git clone https://github.com/tst-race/ext-builder.git
git clone https://github.com/tst-race/ext-cppcheck.git
./ext-builder/build.py \
    --target linux-x86_64 \
    ./ext-cppcheck
```

## Platforms

Cppcheck is built for the following platforms:

* `linux-x86_64`
* `linux-arm64-v8a`

## How It Is Used

Cppcheck is used to perform static analysis on the RACE core source code.
