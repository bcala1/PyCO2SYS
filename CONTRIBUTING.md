# Contributing to PyCO2SYS

Contributions to PyCO2SYS from anyone are very welcome, but please read this first!

## Ideas and bug reporting

If you would like a new feature to be added to PyCO2SYS, or if you find a bug or error in any of its calculations, then please first [share this as an issue](https://github.com/mvdh7/PyCO2SYS/issues). Please do this regardless of whether you are able to solve the issue yourself, to help to avoid duplicate work.

## Adding or editing code

If you would like to add or edit something directly then please make a fork of PyCO2SYS, make your changes, and submit the updates back with a pull request, noting the comments below.  If you are frequently making lots of contributions, you could also be given direct access to the main repo.

Please add a comment on the corresponding [issue](https://github.com/mvdh7/PyCO2SYS/issues) to say that you are working on that problem.

### Branches

The *main* branch contains the most recent release, and nothing more.  Please do not submit pull requests directly to *main*.

The *develop* branch is where the next version is being prepared.  When you have something ready to add, please submit your pull request to *develop*.  You may also wish to make your new fork from *develop* to be sure you are using the latest version.

### Code style

Every module and function must have at least a simple docstring.  I am in the process of updating the docstrings to follow the [numpydoc](https://numpydoc.readthedocs.io/en/stable/format.html) format, so please follow this for any new additions.

Functions that are "private" and not intended to be used by the typical end user should begin with an underscore.  These still require a docstring.

For readable consistency with minimal effort, everything in PyCO2SYS (except for the module `PyCO2SYS.original`, for consistency with its MATLAB predecessor) will be reformatted by [Black](https://black.readthedocs.io/en/stable/?badge=stable) before each new release.

### Credit

Anyone making a substantial contribution will be invited to join the list of authors for the [Zenodo citation](https://doi.org/10.5281/zenodo.3744275).

## Documentation

Documentation is available at [PyCO2SYS.readthedocs.io](https://pyco2sys.readthedocs.io/en/latest/).  This site is automatically generated after each commit from the files in the [docs](https://github.com/mvdh7/PyCO2SYS/tree/main/docs) directory on `main` using [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).  The docs on *develop* are also automatically generated after each commit to that branch and can be seen at [mvdh.xyz/PyCO2SYS](https://mvdh.xyz/PyCO2SYS/).

There is a repo of PyCO2SYS examples as [Jupyter Notebooks](https://jupyter.org/), which you can add to at [PyCO2SYS-examples](https://github.com/mvdh7/PyCO2SYS-examples).

If you add new features to PyCO2SYS, please also propose some sort of documentation for them in one of these formats.

Any changes that you make should be added to appropriate set of release notes in the [version history](https://github.com/mvdh7/PyCO2SYS/blob/develop/docs/versions.md) and any related citations added to the [references](https://github.com/mvdh7/PyCO2SYS/blob/develop/docs/refs.md).

## Roadmap

A very approximate plan of future additions to the code, and the person leading their implementation (get in touch with them to contribute):

### Non-version specific

  * Add validity checker for temperature, salinity and pressure conditions (see https://github.com/mvdh7/PyCO2SYS/issues/25).
  * Integrate with [Pytzer](https://github.com/mvdh7/pytzer) ([mvdh7](https://github.com/mvdh7)).
  
### Things that will not be added

  * Air-sea CO<sub>2</sub> flux calculations.
  * Alkalinity titration solvers - use e.g. [Calkulate](https://github.com/mvdh7/calkulate).
