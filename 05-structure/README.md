## Directory structure

```
hello_app                               Root folder
        ├── app                         Application package
        │   ├── __init__.py             Application factory
        │   ├── hello                   Blueprint
        │   │   ├── __init__.py         Blueprint constructor
        │   │   └── routes.py           Blueprint routes
        │   └── templates               Template folder
        │       └── hello               Blueprint specific templates
        │           └── index.html      Blueprint template
        ├── config_development.py       Development configuration
        ├── config_production.py        Production configuration
        ├── config_testing.py           Unit test package
        ├── manage.py                   Launch script
        └── tests                       Unit tests package
            └── test_basics.py          Basic test cases
```

## Testing

```
MONGO_TEST_URI='mongodb://<user>:<passwd>@oceanic.mongohq.com:10097/<dbname>' FLASK_CONFIG='testing' python manage.py test
```


## Run Server
#### Development Environment

```
MONGO_DEV_URI='mongodb://<user>:<passwd>@oceanic.mongohq.com:10097/<dbname>' python manage.py runserver
```

#### Production Environment

```
MONGO_URI='mongodb://<user>:<passwd>@oceanic.mongohq.com:10097/<dbname>' FLASK_CONFIG='production' python manage.py runserver
```
