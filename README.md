# thing
"thing" python database using dicts [![Codacy Badge](https://api.codacy.com/project/badge/grade/83fa6dc499a54f2c9cf575c14eac6a07)] (https://www.codacy.com/app/me_64/thing) [![PyPI](https://img.shields.io/pypi/dm/Django.svg)](https://pypi.python.org/pypi/thingdb) [![PyPI](https://img.shields.io/pypi/status/Django.svg)](https://pypi.python.org/pypi/thingdb) [![Github All Releases](https://img.shields.io/github/downloads/atom/atom/total.svg)](https://github.com/dev-zz/thing)


usage:

```
import thingdb
secret = "<secret here>"
tdb = thingdb.start("path/to/db.thing", secret)

tdb['demo'] = "Thing is awesome!"

thingdb.save(tdb, "path/to/db.thing", secret)
```

"secret" is a 32 byte string used to decrypt the file; it is optional but must be used every time after used to save it once.

Upon first use you will need to do:

```
import thingdb
secret = "<secret here>"
thingdb.save({}, "path/to/db.thing", secret)
```

installation:

```
git clone https://github.com/dev-zz/thing.git thing
cd thing
python setup.py install
```

https://pypi.python.org/pypi/thingdb


[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/dev-zz/thing/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

