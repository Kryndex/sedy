[![Build Status](https://travis-ci.org/marmelab/sedy.svg?branch=master)](https://travis-ci.org/marmelab/sedy) [![Deps Status](https://david-dm.org/marmelab/sedy.svg)](https://david-dm.org/marmelab/sedy)

# Sedy
A github webhook which helps you to correct your commits

# Install npm dependencies

```bash
make install
```

# Run project

```bash
make run
```

Don't forget to configure your Github webhook to push the **Pull Request review comment** event. All other events will be ignored.

# Configuration

```json
{
    "bot": {
        "login": "GITHUB-ACCOUNT",
        "oauthToken": "GITHUB-OAUTH-ACCESS-TOKEN"
    },
    "committer": {
        "name": "COMMITTER-NAME",
        "email": "an@example.mail"
    },
    "logs": {
        "debug": false
    }
}
```

# Unit-testing

```bash
make test
```

# Deployment

```bash
NODE_ENV=production make deploy
```
