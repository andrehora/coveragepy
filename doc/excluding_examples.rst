.. Licensed under the Apache License: http://www.apache.org/licenses/LICENSE-2.0
.. For details: https://github.com/nedbat/coveragepy/blob/master/NOTICE.txt

.. excluding_examples:

==========================================
Exclusion examples
==========================================

Here's a list of exclusions typically used by open-source projects::

    [report]
    # Regexes for lines to exclude from consideration
    exclude_lines =
        # Have to re-enable the standard pragma
        pragma: no cover

        # Don't complain about missing debug-only code:
        def __repr__
        if self.debug
        if settings.DEBUG

        # Don't complain if tests don't hit defensive assertion code:
        raise AssertionError
        raise NotImplementedError

        # Don't complain if non-runnable code isn't run:
        if 0:
        if False:
        if __name__ == .__main__.:

        # You may also consider to exclude the following exceptions:
        except ImportError
        except AttributeError
        except IOError
        except OSError
        except KeyError
        except ValueError
        except NameError

        # Other possible cases for exclusion that should be customized:
        if sys.platform == 'foo'
        if os.name == 'bar'
        if self.my_legacy_code
        if self.verbose
        def dummy_code


Note that when using regex like ``sys.platform``, ``os.name``, ``self.my_legacy_code``, etc
you should customize the excluded code with your own values.
For example, ``if sys.platform == 'win32'`` or ``if self.use_legacy_matplotlib``.
