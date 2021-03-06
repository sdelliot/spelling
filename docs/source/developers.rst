.. spelling::

   sphinxcontrib
   reStructuredText

============
 Developers
============

If you would like to contribute to sphinxcontrib.spelling directly,
these instructions should help you get started.  Patches, bug reports,
and feature requests are all welcome through the `GitHub site
<https://github.com/sphinx-contrib/spelling>`__.
Contributions in the form of patches or pull requests are easier to
integrate and will receive priority attention.

Running tests
=============

To run the tests, you need ``tox`` installed, then just run
``tox``. This should run the unit tests, the source code linter, and
try to build the current documentation.

Building Documentation
======================

The documentation for sphinxcontrib.spelling is written in
reStructuredText and converted to HTML using Sphinx. The build is
driven by ``tox``. To build only the documentation, run ``tox -e
docs``.

Contributing
============

Please submit changes as pull requests using the `GitHub repository
<https://github.com/sphinx-contrib/spelling>`__.

In the pull request description, link to any issues closed by the
changes using ``Fixes #NUM``, replacing ``NUM`` with the issue number.

Release Notes
=============

Please use reno_ to add a release note for each pull request.

.. code-block:: console

   $ tox -e docs
   $ .tox/docs/bin/reno new slug
   # edit file created by reno

Refer to the reno_ documentation for more details.

.. _reno: https://docs.openstack.org/reno/latest/
