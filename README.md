# BlueDoc

[![Build Status](https://travis-ci.org/thebluedoc/bluedoc.svg?branch=master)](https://travis-ci.org/thebluedoc/bluedoc) [![codecov](https://codecov.io/gh/thebluedoc/bluedoc/branch/master/graph/badge.svg)](https://codecov.io/gh/thebluedoc/bluedoc)


## Development

You need install depends softwares first:

```bash
$ brew install node imagemagick postgresql elasticsearch redis
$ brew cask install wkhtmltopdf
```

Setup the default ENV vars to open all features:

```
export LDAP_HOST=localhost

export OMNIAUTH_GOOGLE_CLIENT_ID=
export OMNIAUTH_GOOGLE_CLIENT_SECRET=

export OMNIAUTH_GITHUB_CLIENT_ID=
export OMNIAUTH_GITHUB_CLIENT_SECRET=

export OMNIAUTH_GITLAB_CLIENT_ID=
export OMNIAUTH_GITLAB_CLIENT_SECRET=
export OMNIAUTH_GITLAB_API_PREFIX=
```

Start development server:

- `yarn start` - to start webpack dev server.
- `rails s` - to start rails

```bash
$ yarn start
```

In other Termal tab:

```bash
$ rails s
```

## Install plantuml-service

plantuml-service for generate PlantUML image

https://github.com/bitjourney/plantuml-service

```bash
$ brew install bitjourney/self/plantuml-service
$ brew services start bitjourney/self/plantuml-service
```

### Generate Admin

```bash
$ rails g scaffold_controller admin/repository slug:string name:string user:references description:string
```
