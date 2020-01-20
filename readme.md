Flask Full Text Search with nearby search using Postgres and PostGIS
---
0. Activate virtualenv

1. `pip3 install -r requirements.txt`

2. Change  `SQLALCHEMY_DATABASE_URI` to your psql db credentials

3. run before you start
```
python app.py shell
from app import db
from sqlalchemy.orm.mapper import configure_mappers
configure_mappers()
db.create_all()
exit()
```

4. Insert test data
```
psql shell
INSERT INTO document ("title" , "description")
        VALUES ("casa" , "es roja con techo verde")

...
```
5. `python app.py runserver`




