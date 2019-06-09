INSTALLATION
============

Setup the buildout cache
------------------------

```bash
mkdir ~/.buildout
cd ~/.buildout
mkdir eggs
mkdir downloads
mkdir extends
echo "[buildout]
eggs-directory = /home/cmrs/.buildout/eggs
download-cache = /home/cmrs/.buildout/downloads
extends-cache = /home/cmrs/.buildout/extends" > ~/.buildout/default.cfg
```

Download the buildout and create the venv
-----------------------------------------

```bash
git clone git@github.com:cmrs/buildout.cmrs.git <venv_folder>
cd <venv_folder>
virtualenv .
```

Install and initialise buildout
-------------------------------

```bash
pip install zc.buildout
buildout init
```

Run the buildout
----------------

```bash
buildout -c default.cfg
```
