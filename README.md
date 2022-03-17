# Django GraphiQL Strawberry Debug Toolbar

[![Tests](https://github.com/przemub/django-graphiql-strawberry-debug-toolbar/actions/workflows/test-suite.yml/badge.svg)](https://github.com/flavprzemub/django-graphiql-strawberry-debug-toolbar/actions)
[![Package version](https://img.shields.io/pypi/v/django-graphiql-strawberry-debug-toolbar.svg)](https://pypi.python.org/pypi/django-graphiql-strawberry-debug-toolbar)

[Django Debug Toolbar](https://github.com/jazzband/django-debug-toolbar) for [GraphiQL](https://github.com/graphql/graphiql) IDE and [Strawberry](https://strawberry.rocks/) GraphQL server.

![Graphiql Debug Toolbar](https://user-images.githubusercontent.com/5514990/36340937-1937ee68-1419-11e8-8477-40622e98c312.gif)

## Dependencies

* Python ≥ 3.7
* Django ≥ 2.2
* Strawberry ≥ 0.15.1

## Installation

Install the last stable version from PyPI.

```sh
pip install django-graphiql-strawberry-debug-toolbar
````

See the [documentation](https://django-debug-toolbar.readthedocs.io/en/stable/installation.html) for further guidance on setting *Django Debug Toolbar*.

Add `graphiql_strawberry_debug_toolbar` to your *INSTALLED_APPS* settings:

```py
INSTALLED_APPS = [
    'debug_toolbar',
    'graphiql_strawberry_debug_toolbar',
]
```

**Replace** the Django Debug Toolbar **middleware** with the GraphiQL Debug Toolbar one. 

```py
MIDDLEWARE = [
    # 'debug_toolbar.middleware.DebugToolbarMiddleware',
    'graphiql_strawberry_debug_toolbar.middleware.DebugToolbarMiddleware',
]
```

Credits to [@jazzband](https://jazzband.co) / [django-debug-toolbar](https://github.com/jazzband/django-debug-toolbar)
 and [@mongkok](https://github.com/mongkok), the author of [the orignal tool](https://github.com/flavors/django-graphiql-debug-toolbar) for graphene.

