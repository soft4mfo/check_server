# Check server deployment
To deploy config you need to add two .env files for fssp and passport services.

##### fssp.env
```env
#Django settings
SECRET_KEY=
RUCAPTCHA_API_KEY=
SERVICE_TOKEN=
DEBUG=0

#Postgres settings
POSTGRES_DB=check_db
POSTGRES_USER=checkdbuser
POSTGRES_PASSWORD=
POSTGRES_HOST=db

#Reverse-proxy settings
DEFAULT_EMAIL=
VIRTUAL_HOST=
LETSENCRYPT_HOST

```

##### passport.env
```env
#Django settings
PASSPORT_SECRET_KEY=
PASSPORT_SERVICE_TOKEN=

PGDATA=/var/lib/postgresql/data/pgdata
C_FORCE_ROOT=true

#Postgres settings
PASSPORT_DB=passport_db
POSTGRES_DB=passport_db
POSTGRES_USER=passportdbuser
POSTGRES_PASSWORD=
POSTGRES_HOST=db_passport

#Reverse-proxy settings
DEFAULT_EMAIL=
VIRTUAL_HOST=
LETSENCRYPT_HOST

```
