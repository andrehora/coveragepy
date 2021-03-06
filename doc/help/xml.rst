
.. code::

    $ coverage xml --help
    Usage: coverage xml [options] [modules]

    Generate an XML report of coverage results.

    Options:
      --fail-under=MIN      Exit with a status of 2 if the total coverage is less
                            than MIN.
      -i, --ignore-errors   Ignore errors while reading source files.
      --include=PAT1,PAT2,...
                            Include only files whose paths match one of these
                            patterns. Accepts shell-style wildcards, which must be
                            quoted.
      --omit=PAT1,PAT2,...  Omit files whose paths match one of these patterns.
                            Accepts shell-style wildcards, which must be quoted.
      -o OUTFILE            Write the XML report to this file. Defaults to
                            'coverage.xml'
      --skip-empty          Skip files with no code.
      --debug=OPTS          Debug options, separated by commas. [env:
                            COVERAGE_DEBUG]
      -h, --help            Get help on this command.
      --rcfile=RCFILE       Specify configuration file. By default '.coveragerc',
                            'setup.cfg', 'tox.ini', and 'pyproject.toml' are
                            tried. [env: COVERAGE_RCFILE]

