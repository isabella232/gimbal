# Gimbal `audit` Command

The `audit` command, by default, runs the [`heap-snapshot`](../../module/heap-snapshot), [`lighthouse`](../../module/lighthouse), [`size`](../../module/size) and [`unused-source`](../../module/unused-source) modules aimed for an application generated by the [create-react-app](https://facebook.github.io/create-react-app/) tool.

## Usage

To use, simply execute `gimbal audit` in the root of your `create-react-app` generated project.

**NOTE** You should build the project prior to running Gimbal on it as this will test the built application.

## Options

You can opt-out of running a module via these cli flags:

- `--no-heap-snapshot` Disabled the `heap-snapshot` module.
- `--no-lighthouse` Disabled the `lighthouse` module.
- `--no-size` Disabled the `size` module.
- `--no-calculate-unused-source` Disabled the `unused-source` module.

The following are other options:

- `--build-dir [dir]` By default, the build directory is specified as `build` but you can change it. This path is relative to the current working directory.
- `--no-check-thresholds` by default, Gimbal will check values against thresholds. Setting this option will disable threshold checks.
