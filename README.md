# ![xleaflet](docs/source/xleaflet.svg)

[![Travis](https://travis-ci.org/QuantStack/xleaflet.svg?branch=master)](https://travis-ci.org/QuantStack/xleaflet)
[![Appveyor](https://ci.appveyor.com/api/projects/status/gfiivu33g6hrv220?svg=true)](https://ci.appveyor.com/project/QuantStack/xleaflet)
[![Documentation](http://readthedocs.org/projects/xleaflet/badge/?version=latest)](https://xleaflet.readthedocs.io/en/latest/?badge=latest)
[![Binder](https://img.shields.io/badge/launch-binder-brightgreen.svg)](https://mybinder.org/v2/gh/QuantStack/xleaflet/stable?filepath=notebooks)
[![Join the Gitter Chat](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/QuantStack/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

C++ backend for the jupyter-leaflet map visualization library

## Usage

Selecting a base layer for a map:

![Basemap Screencast](basemap.gif)

Loading a geojson dataset:

![GeoJSON Screencast](geojson.gif)

Using the splitmap control:

![Splitmap Screencast](splitmap.gif)

Displaying velocity data on the top of a map:

![Velocity Screencast](velocity.gif)

## Installation

We provide a package for the conda package manager.

- Installing `xleaflet` and the C++ kernel

```bash
conda install xeus-cling xleaflet -c QuantStack -c conda-forge
```

Then, the front-end extension must be installed for either the classic notebook or JupyterLab.

- Installing the extensions for the classic notebook

```
conda install widgetsnbextension -c conda-forge
conda install ipyleaflet -c conda-forge
```

- Installing the JupyterLab extension

```
jupyter labextension install @jupyter-widgets/jupyterlab-manager
jupyter labextension install jupyter-leaflet
```

## Installation from sources

Or you can directly install it from the sources if you have all the dependencies already installed:

```bash
cmake -D CMAKE_INSTALL_PREFIX=your_install_prefix
make install
```

## Trying it online

To try out xleaflet interactively in your web browser, just click on the binder
link:

[![Binder](docs/source/binder-logo.svg)](https://mybinder.org/v2/gh/QuantStack/xleaflet/stable?filepath=notebooks/)

## Documentation

To get started with using `xleaflet`, check out the full documentation

http://xleaflet.readthedocs.io/

## Dependencies

All the dependencies of xleaflet are available for the conda package manager.

| `xleaflet` | `xwidgets`  |  `xeus`         |  `xtensor`      |  
|------------|-------------|-----------------|-----------------|
|  master    |   ~0.18.0   |  >=0.20.0,<0.21 |  >=0.20.8,<0.21 |
|  0.8.0     |   ~0.18.0   |  >=0.20.0,<0.21 |  >=0.20.8,<0.21 |
|  0.7.0     |   ~0.17.0   |  >=0.19.1,<0.20 |  >=0.20.1,<0.21 |
|  0.6.1     |   ~0.16.1   |  >=0.18.1,<0.19 |  >=0.19.1,<0.20 |
|  0.6.0     |   ~0.16.0   |  >=0.18.1,<0.19 |  >=0.19.1,<0.20 |
|  0.5.0     |   ~0.15.0   |  >=0.17.0,<0.18 |  >=0.19.0,<0.20 |
|  0.4.0     |   ~0.14.0   |  >=0.15.0,<0.16 |  >=0.18.1,<0.19 |
|  0.3.1     |   ~0.13.1   |  >=0.14.1,<0.15 |                 |
|  0.3.0     |   ~0.13.0   |  >=0.13.0,<0.14 |                 |
|  0.2.1     |   ~0.12.2   |  >=0.13.0,<0.14 |                 |
|  0.2.0     |   ~0.12.0   |  >=0.13.0,<0.14 |                 |
|  0.1.0     |   ~0.10.0   |  >=0.12.0,<0.13 |                 |
|  0.0.1     |   ~0.9.0    |  >=0.12.0,<0.13 |                 |

## License

We use a shared copyright model that enables all contributors to maintain the
copyright on their contributions.

This software is licensed under the BSD-3-Clause license. See the [LICENSE](LICENSE) file for details.
