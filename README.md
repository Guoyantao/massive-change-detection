# Massive Change Detection - QGIS plugin

QGIS 2 plugin that applies change detection algorithms on satellite imagery for
building reports for urban planning.


## Install

...


## Usage

### Generate change detection raster

...

### Build report of changes

...


## Development

Clone the repository inside QGIS plugin directory.  On Ubuntu this would be
`~/.qgis2/python/plugins/`:

```
cd ~/.qgis2/python/plugins/
git clone https://github.com/dymaxionlabs/massive-change-detection
cd massive-change-detection
```

Install packages for test and code coverage.

```
pip install --user -r requirements.txt
pip install --user -r requirements-dev.txt
```

If you have installed QGIS from source use `scripts/run-env-linux.sh` to set up
the environment variables so that Python can find QGIS inside your virtual
environment.  For example, if it is `/opt/qgis2`:

```
source scripts/run-env-linux.sh /opt/qgis2
```

Run tests and build code coverage reports with `make test`.

### I18n

You can find the list of supported locales is in the `LOCALES` definition on
`Makefile`. If you want to add a new language, you have to add it there first.

Prepare translations strings with `make transup`. This command will search all
translated strings in the repository and generate `.ts` files.

Edit the translations files (files ending in `.ts`) in `i18n/`.

Finally compile translation strings with `make transcompile`.


## Issue tracker

Please report any bugs and enhancement ideas using the GitHub issue tracker:

  https://github.com/dymaxionlabs/massive-change-detection/issues

Feel free to also ask questions on our [Gitter
channel](https://gitter.im/dymaxionlabs/massive-change-detection), or by email.


## Help wanted

Any help in testing, development, documentation and other tasks is highly
appreciated and useful to the project.

For more details, see the file [CONTRIBUTING.md](CONTRIBUTING.md).


## License

Source code is released under a GNU GPL v3 license.  Please refer to
[LICENSE.md](LICENSE.md) for more information.
