Flask Full Text Search with nearby search using Postgres and PostGIS
---

1. `pip install -r requirements.txt`

2. Change `SQLALCHEMY_DATABASE_URI`

3. run before you start
```
from app import db
from sqlalchemy.orm.mapper import configure_mappers
configure_mappers()
db.create_all()
```

4. `python app.py`

Test data
```
psql shell
INSERT INTO document ("title" , "description")
        VALUES ("casa" , "es roja con techo verde")
...



