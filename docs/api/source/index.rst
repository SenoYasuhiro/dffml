Sources
=======

Sources are how DFFML abstracts storage of feature data. This allows users to
swap out their data sources as they progress from testing through integration.

Most DFFML CLI commands work with the :class:`dffml.source.source.Sources` class
which merges the feature data of Repos with the same ``src_url``. This means
when multiple sources are given to those CLI commands, feature data stored in
those various sources/databases under the same unique key will automatically
accessible within one :class:`dffml.repo.Repo`.

DFFML has several built in sources which can be used programmatically or via the
CLI and other services.

.. toctree::
    :glob:
    :maxdepth: 2
    :caption: Contents:

    base
    memory
    file
