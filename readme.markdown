This is a log. 2015-10-30. 0900 hours.

Virtualenv, python 2.
`virtualenv --system-site-packages --python=python2.7 pyenv`

Pip install pip, fiona, shapely.

Was working with the SA2012VT files, those are VT parks.
Downloaded national parks from https://irma.nps.gov/App/Reference/DownloadDigitalFile?code=530102&file=nps_boundary.zip

Hm, works fine without speedups but seems slow (couldn't get through the 15 minutes of tweets that I downloaded).
With speedups, looks like it's using GEOS under the hood, but doesn't accept the geometry.

Installed gdal with homebrew, which install geos, but no change.
Maybe it will just work on the VACC with those binaries.
And it does.

Would likely have to build from source to get speedups working on the Mac.
