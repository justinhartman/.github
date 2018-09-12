# .github

A set of Github templates that accelerate your project setup and
configuration.

### Table of Contents

- [Overview](#overview)
- [Screenshots](#screenshots)
  - [Github Issues](#github-issues)
  - [Github Issue - General Report](#github-issue---general-report)
  - [Github Issue - Feature Request](#github-issue---feature-request)
  - [Github Issue - Bug Report](#github-issue---bug-report)
  - [Github Pull Request](#github-pull-request)
- [Installing](#installing)
  - [Clone the repository to your machine](#clone-the-repository-to-your-machine)
  - [Copying the main project structure](#copying-the-main-project-structure)
  - [Copying only some of the project structure](#copying-only-some-of-the-project-structure)
  - [Choosing and Copying a License file](#choosing-and-copying-a-license-file)
  - [The Final Structure](#the-final-structure)
  - [File Changes](#file-changes)
- [Authors](#authors)
- [License](#license)
- [Contributing](#contributing)
- [Code of Conduct](#code-of-conduct)
- [Versioning](#versioning)
- [Change-Log](#change-log)
- [Acknowledgements](#acknowledgements)

## Overview

Everything you need is contained within the `/templates/` folder. This
includes all the files needed to start a project from scratch, which include:

- `.github/` folder with templates for working with Github's `Issue` and
  `Pull Request`. See [the screenshots below][screenshots] for how these
  integrate directly with Github.
- `.gitignore` file to ignore certain files and folders.
- `CHANGELOG.md` file provides a template for tracking releases and changes.
- `CODE_OF_CONDUCT.md` file which governs your project.
- `CONTRIBUTING.md` file outlining how contributors can get involved.
- `README.md` file which is thorough and can be tailored to your needs.
- `_licenses/` folder containing all available open-source licenses.

The below output is the full file list of the `/templates/` folder.

```terminal
templates/
├── _core/
│   ├── .github/
│   │   ├── ISSUE_TEMPLATE/
│   │   │   ├── BUG_REPORT.md
│   │   │   ├── CUSTOM.md
│   │   │   └── FEATURE_REQUEST.md
│   │   └── PULL_REQUEST_TEMPLATE.md
│   ├── .gitignore
│   ├── CHANGELOG.md
│   ├── CODE_OF_CONDUCT.md
│   ├── CONTRIBUTING.md
│   └── README.md
└── _licenses/
    ├── afl-3.0.txt
    ├── agpl-3.0.txt
    ├── apache-2.0.txt
    ├── artistic-2.0.txt
    ├── bsd-2-clause.txt
    ├── bsd-3-clause-clear.txt
    ├── bsd-3-clause.txt
    ├── bsl-1.0.txt
    ├── cc-by-4.0.txt
    ├── cc-by-sa-4.0.txt
    ├── cc0-1.0.txt
    ├── ecl-2.0.txt
    ├── epl-1.0.txt
    ├── epl-2.0.txt
    ├── eupl-1.1.txt
    ├── eupl-1.2.txt
    ├── gpl-2.0.txt
    ├── gpl-3.0.txt
    ├── isc.txt
    ├── lgpl-2.1.txt
    ├── lgpl-3.0.txt
    ├── lppl-1.3c.txt
    ├── mit.txt
    ├── mpl-2.0.txt
    ├── ms-pl.txt
    ├── ms-rl.txt
    ├── ncsa.txt
    ├── ofl-1.1.txt
    ├── osl-3.0.txt
    ├── postgresql.txt
    ├── unlicense.txt
    ├── upl-1.0.txt
    ├── wtfpl.txt
    └── zlib.txt
```

## Screenshots

The screenshots below demonstrate how the files contained in the `.github/`
folder integrate with Github's `Issue` and `Pull Request` features. As you
will see, each template allows you to have a unique template when logging
Issues or creating a Pull Request.

### Github Issues

![Github Issues][screen-1]

### Github Issue - General Report

![General Report][screen-2]

### Github Issue - Feature Request

![Feature Request][screen-3]

### Github Issue - Bug Report

![Bug Report][screen-4]

### Github Pull Request

![Pull Request][screen-5]

## Installing

### Clone the repository to your machine

First off you want to clone the repository to your local machine. You can do
so by running the following commands in a terminal.

```terminal
$ git clone https://github.com/justinhartman/.github github-templates
$ cd github-templates/
```

**NB:*- Specifying a name for the checkout folder (e.g. `github-templates`)
when running `git clone` is very important. If you don't, `git` will checkout
the repo to a folder called `.github` on your local machine. If you are using
`macOS` or `Linux` you won't be able to see the newly checked out repo due to
the fact it begins with a period (`.`) and will be hidden by the file-system.
It is there; you just cannot see it without running something like `ls -la`.

### Copying the main project structure

To copy the main project structure for a new project simply execute the
following commands from the repository root folder.

```terminal
$ cd templates/
$ cp -R _core/ /path/to/your/project/folder/ # change path to your project
```

This will copy all the files from the `_core/` folder into your project root
folder. Your project will now contain the following files:

```terminal
/path/to/your/project/folder/
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   ├── BUG_REPORT.md
│   │   ├── CUSTOM.md
│   │   └── FEATURE_REQUEST.md
│   └── PULL_REQUEST_TEMPLATE.md
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
└── README.md
```

### Copying only some of the project structure

You may not want to copy everything contained in the `_core/` folder;
especially if you've already initiated a `git` repo (i.e. `git init`) and have
a `.gitignore` and/or `README.md` file already contained in your project path.

Copying only _some_ of the main project structure files can be achieved by
running the following commands.

```terminal
$ cd templates/_core/
$ cp -R .github .gitignore CHANGELOG.md CODE_OF_CONDUCT.md \
   CONTRIBUTING.md README.md \
     /path/to/your/project/folder/ # change path to your project
```

You can simply remove the file(s) and/or `.github` folder from the above `cp`
command thereby copying only the files/folder you need. For example, the below
will copy everything _except_ the `README.md` and `.gitignore` files.

```terminal
$ cp -R .github CHANGELOG.md CODE_OF_CONDUCT.md CONTRIBUTING.md \
  /path/to/your/project/folder/ # change path to your project
```

### Choosing and Copying a License file

The `_licenses` folder contains a collection of largely most of the
open-source licenses available. To copy a license, choose one from the folder
and run the following from your terminal.

```terminal
$ cd templates/_licenses/
$ cp mit.txt /path/to/your/project/folder/LICENSE # change path to your project
                                                  # but leave LICENSE intact
```

**NB:*- make sure that when you copy a license file you always name your
license as `LICENSE` and not, for example, `mit.txt`. Github looks for a file
called `LICENSE` in the root of your project folder so anything other than
this and Github won't be able to figure out what license your project is
under.

### The Final Structure

Once you have copied across the basic project structure and a license file you
should end up with your project directory looking like this:

```terminal
/path/to/your/project/folder/
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   ├── BUG_REPORT.md
│   │   ├── CUSTOM.md
│   │   └── FEATURE_REQUEST.md
│   └── PULL_REQUEST_TEMPLATE.md
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
└── README.md
```

### File Changes

These templates have been designed to work _out-the-box_ without much need for
intervention on your part. There are however a few files where you will need
to make some changes in order to tailor this to your project. See below for a
list of changes you **should make*- before committing to your repo.

As a recommendation, it is better to edit the files in your project folder
rather than in this repository. This will allow you to update the repo without
losing any changes you may have made.

- `/.gitignore` - this template has been configured to ignore file-system
  specific files for macOS, Windows and Linux. Delete whatever is not
    relevant to your needs.
- `/CHANGELOG.md` - update your versioning structure and enter a release date.
- `/README.md` - you will make many changes to this file but you must update
  the URLs at the end of the file. Currently they link to this repo and should
    be replaced with your Github project URL.
- `/CONTRIBUTING.md` - as with the `README.md` you need to update the links
  to your project at the end of the file.
- `/CODE_OF_CONDUCT.md` - at the end of this file you will need to replace the
  generic email address with an email address for your project.

## Authors

- Justin Hartman - [@justinhartman][author-1]

Also see the list of [contributors][contribs] who have participated in this
project.

## License

This project is licensed under the `AGPL-3.0` License. See the
[LICENSE][license] file for full details.

```text
Copyright (C) 2018 Justin Hartman <justin@hartman.me>.

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Affero General Public License as
published by the Free Software Foundation, either version 3 of the
License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License
along with this program. If not, see <https://www.gnu.org/licenses/>.
```

## Contributing

Please read the [CONTRIBUTING.md][CONTRIBUTING] file for details on how you
can get involved in the project as well as the process for submitting bugs
and pull requests.

## Code of Conduct

Please read the [CODE_OF_CONDUCT.md][COC] file for the guidelines that govern
the community.

## Versioning

We use [Semantic Versioning][semver] for software versions of this project.
For a list of all the versions available, see the [tags][tags] and
[releases][releases] on this repository.

## Change-Log

View the [`CHANGELOG.md`][changelog] file for a detailed list of changes,
along with specific tasks completed for each version released to date.

## Acknowledgements

Special thanks go out to the following people and projects who have helped in
some way to make this project a reality.

- [@daniellmb/.github][daniellmb] - for the original idea to create a
  `.github` template pack.
- [PurpleBooth/README-Template.md][purple-booth] - for the README file
  inspiration.
- [Github][github-link] - for the `ISSUE_TEMPLATE` template files.

[screenshots]: #screenshots
[email]: mailto:justin@hartman.me?subject=Github+Contact
[license]: LICENSE
[site]: https://justin.hartman.me
[post]: https://justin.hartman.me
[git]: https://github.com/justinhartman/.github
[github]: https://github.com/justinhartman/.github/issues
[purple-booth]: https://gist.github.com/PurpleBooth/109311bb0361f32d87a2
[CONTRIBUTING]: CONTRIBUTING.md
[COC]: CODE_OF_CONDUCT.md
[semver]: http://semver.org
[tags]: https://github.com/justinhartman/.github/tags
[releases]: https://github.com/justinhartman/.github/releases
[contribs]: https://github.com/justinhartman/.github/contributors
[author-1]: https://github.com/justinhartman
[github-link]: https://github.com/github
[screen-1]: https://ws1.sinaimg.cn/large/006tKfTcly1fr6nlcwl2xj30lx08gmxm.jpg
[screen-2]: https://ws3.sinaimg.cn/large/006tKfTcly1fr6nmfm23gj30lt0j00un.jpg
[screen-3]: https://ws2.sinaimg.cn/large/006tKfTcgy1fr6nqbp7n3j30lk0f5wgg.jpg
[screen-4]: https://ws4.sinaimg.cn/large/006tKfTcgy1fr6nrhrn19j30lm136jut.jpg
[screen-5]: https://ws1.sinaimg.cn/large/006tKfTcgy1fr6nrov8hbj30lg0vlq5o.jpg
[daniellmb]: https://github.com/daniellmb/.github
[changelog]: CHANGELOG.md
