# hydrogen-run

A superset of commands to improve hydrogen workflow.

> [!NOTE]
> This package is in maintenance mode. If you use [Lumine](https://github.com/lumine-code/lumine), you may be interested in [jupyter-cells](https://github.com/lumine-code/jupyter-cells) and [jupyter-repl](https://github.com/lumine-code/jupyter-repl).

![demo](https://github.com/asiloisad-pulsar/hydrogen-run/blob/master/assets/demo.gif?raw=true)

Consider to use [hydrogen-next](https://github.com/asiloisad-pulsar/hydrogen-next) or [jupyter-next](https://github.com/asiloisad-pulsar/jupyter-next) instead.

## Installation

To install `hydrogen-run` search for [hydrogen-run](https://web.pulsar-edit.dev/packages/hydrogen-run) in the Install pane of the Pulsar settings or run `ppm install hydrogen-run`. Alternatively, you can run `ppm install asiloisad-pulsar/hydrogen-run` to install a package directly from the GitHub repository.

Requires [hydrogen-next](https://github.com/asiloisad-pulsar/hydrogen-next) or [hydrogen](https://github.com/nteract/hydrogen).

## Commands

Commands available in `atom-text-editor:not([mini])`:

- `hydrogen:run-all`: push all text in single run,
- `hydrogen-run:recalculate-all`: clear results, reset kernel and push all text in single run,
- `hydrogen:run-all-above`: push above text in single run,
- `hydrogen-run:recalculate-all-above`: clear results, reset kernel and push above text in single run,
- `hydrogen-run:run-all-inline`: push all text in multiple runs,
- `hydrogen-run:recalculate-all-inline`: clear results, reset kernel and push all text in multiple runs,
- `hydrogen-run:run-all-above-inline`: push above text in multiple runs,
- `hydrogen-run:recalculate-all-above-inline`: clear results, reset kernel and push above text in multiple runs,
- `hydrogen:run`: run single statement in single run,
- `hydrogen:run-cell`: run cell in single run,
- `hydrogen:clear-and-center`: clear results and scroll text editor to cursor,
- `hydrogen:interrupt-kernel`: interrupt kernel,
- `hydrogen:run-and-move-down`: run single statement and go to next statement,
- `hydrogen:run-cell-and-move-down`: run single cell and go to next cell,
- `hydrogen-run:clear-and-restart`: clear results and restart kernel,
- `hydrogen:shutdown-kernel`: shutdown kernel,
- `hydrogen:toggle-inspector`: toggle inspector pane.

## New concepts

The package introduce two new concepts of evaluation:

- `recalculate`: clear result -> restart kernel -> run calculation,
- `inline`: calculation is going one breakpoint after one instead of pushing all text to python interpreter instantly. This way you got result next to breakpoints. Inline methods inherit all limitations of hydrogen package, e.g. in Python `if ... else ...` is broken.

## Contributing

Got ideas to make this package better, found a bug, or want to help add new features? Just drop your thoughts on GitHub. Any feedback is welcome!
