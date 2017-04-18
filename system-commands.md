# System commands

- [Introduction](#introduction)
- [Invitation](#invitation)
	- [Usage](#invitation-usage)
- [Documentation](#documentation)
	- [Usage](#documentation-usage)

<a name="introduction"></a>
## Introduction

Commands are used to controll some parts of Yap application from command-line. Commands leverage Artisan command-line interface.

> Artisan is the command-line interface included with Laravel. It provides a number of helpful commands that can assist you while you build your application.

You can always pass some options along with command itself:

| option             | short       | description                         |
|--------------------|-------------|-------------------------------------|
| `--help`           | `-h`        | display help message                |
| `--quiet`          | `-q`        | do not output any message           |
| `--no-interaction` | `-n`        | do not ask any interactive question |
| `--verbose`        | `-v|vv|vvv` | increase the verbosity of messages  |

<a name="listing"></a>
## Invitation

Creates an invitation and sends notifying email.

<a name="invitation-usage"></a>
### Usage

Execute following command, where parameter `<email>` is required.

```bash
$ php artisan yap:invitation <email>
```

| option           | short | description                                             |
|------------------|-------|---------------------------------------------------------|
| `--admin`        | `-a`  | make user also an administrator                         |
| `--force-resend` | `-f`  | force resending an email                                |
| `--indefinite`   | `-i`  | make an invitation valid indefinitely (until signed in) |
| `--dont-send`    | `-d`  | suppress all emails                                     |

> {note} Suppressing emails takes precedence over force resending emails.

#### Example (shorten)

In following example system creates an invitation that is indefinitely valid (in regards of time), sends email to **mr.dean@stuba.sk** and outputs invitation (registration) link to command line. 

```bash
$ php artisan yap:invitation --indefinite mr.dean@stuba.sk
```
Command line output
```markup
Invitation for potential user with email 'mr.dean@stuba.sk' was created.
Invitation link:
http://yap.dev/auth/register/M1lhd2FTR1RHZGN0bTZa...
```

<a name="listing"></a>
## Documentation

Installing or downloading newest version of documentation (user guide).

> {note} Documentation updates itself upon receiving web-hook from GitHub.

<!-- > {github} GitHub [repository](https://github.com/stu-ba/yap-3-user-guide) where documentation is stored. Feel free to fork it and improve it. -->

<a name="documentation-usage"></a>
### Usage

Execute following command with either `--install` or `--update` option.

```bash
$ php artisan yap:docs
```

| option      | short | description                                                 |
|-------------|-------|-------------------------------------------------------------|
| `--install` | `-i`  | install documentation from repository                       |
| `--update`  | `-u`  | update newest documentation from repository (performs pull) |
