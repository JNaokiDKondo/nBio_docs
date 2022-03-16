# TOPAS-nBio
The nanometer scale extension for radiobiology of the TOPAS Monte Carlo system

.. figure:: images/nBio_Logo.png
   :scale: 60 %
.. figure:: images/nBio_Logo.png
   :scale: 60 %

The documentation is written in reStructuredText format (reST). It is hosted by ReadTheDocs. A good resource on reST is the Sphinx documentation, but please note that not all features described there are supported by ReadTheDocs. It also describes some Python-only features, since that is its domain.

If working on a Mac, I recommend installing Python with Homebrew to avoid messing up your system Python.

To build and view the docs locally (recommended for substantial editing), you will need to have Spinx version 1.4.2 or newer and do:

pip install sphinx sphinx-autobuild sphinx_rtd_theme

To install TOPAS pygments:
pip install -e git://github.com/davidchall/topas-pygments.git#egg=topas_pygments

Or in newer versions do:
mkdir src
cd src
git clone https://github.com/davidchall/topas-pygments
cd topas-pygments
python3 setup.py install

then, after your edits

make clean
make html
open .build/html/index.html

If you need a .rst renderer you can use http://rst.ninjs.org/ for quick visualisation.
