## Environments Variables

Autoload Enviroment variables from a `.env` file in the root of the project with the expected variables in [vars.env](../vars.env) file.

| variable     | defaut        | description                                             |
| ------------ | ------------- | ------------------------------------------------------- |
| TMI_TOKEN    |               | the client secret of the bot                            |
| BEARER_ID    |               | the clientid of the bot                                 |
| BOT_NICK     |               | the chatbot name                                        |
| BOT_PREFIX   | "!"           | the prefix for commands                                 |
| CHANNEL      |               | the channel the chatbot will join in                    |
| *MUSIC_PATH* |               | the path containing genre subdirectories with the songs |
| ENVIRONMENT  | "development" | one of "develpment" "production"                        |

---
## pipenv Package Manager
Uses [pipenv](https://github.com/pypa/pipenv) to manage dependencies with the generated `Pipfile`.

see [installing pipenv](https://github.com/pypa/pipenv#installation).

### Installing all packages
```bash
pipenv install
```

### Checking security vulnerabilities
```bash
pipenv check
```

### Generating [requirements.txt](../requirements.txt)
```bash
pipenv lock -r > requirements.txt
```

### activate project's virtualenv
```bash
pipenv shell
```
### Running the project
```bash
pipenv run python mpdbot.py
```
or using the shortcut:
```bash
pipenv run start
```

---