# .github

A set of Github templates that accelerate your project setup and 
configuration.

## Table of Contents
<!-- MarkdownTOC -->

- [Overview](#overview)
- [Installing](#installing)
- [Screenshots](#screenshots)
  - [Github Issues](#github-issues)
  - [Github Issue - General Report](#github-issue---general-report)
  - [Github Issue - Feature Request](#github-issue---feature-request)
  - [Github Issue - Bug Report](#github-issue---bug-report)
  - [Github Pull Request](#github-pull-request)
- [Authors](#authors)
- [License](#license)
- [Contributing](#contributing)
- [Code of Conduct](#code-of-conduct)
- [Versioning](#versioning)
- [Acknowledgements](#acknowledgements)

<!-- /MarkdownTOC -->

## Overview

Everything you need is contained within the `/templates/` folder. This 
includes all the files needed to start a project from scratch, which include:

- `.github/` folder with templates for working with Github's `Issue` and 
  `Pull Request`. See [the screenshots below][screenshots] for how these 
  integrate with Github.
- `.gitignore` file to ignore certain files and folders.
- `CODE_OF_CONDUCT.md` file which governs your project.
- `CONTRIBUTING.md` file outlining how contributors can get involved.
- `README.md` file which is very basic and can be tailored to your needs.
- `_licenses/` folder containing all available open-source licenses.

This is the full file breakdown of the `/templates/` folder.

```terminal
templates/
├── _basic/
│   ├── .github/
│   │   ├── ISSUE_TEMPLATE/
│   │   │   ├── BUG_REPORT.md
│   │   │   ├── CUSTOM.md
│   │   │   └── FEATURE_REQUEST.md
│   │   └── PULL_REQUEST_TEMPLATE.md
│   ├── .gitignore
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

## Installing

## Screenshots

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

## Authors

* Justin Hartman - [@justinhartman][author-1]

Also see the list of [contributors][contribs] who have participated in this 
project.

## License

```
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

Please read our [CONTRIBUTING.md][CONTRIBUTING] file for details on how you 
can get involved in the project as well as the process for submitting bugs 
and pull requests to us.

## Code of Conduct

Please read our [CODE_OF_CONDUCT.md][COC] file for the guidelines that govern 
our community.

## Versioning

We use [Semantic Versioning][semver] for software versions of this project. 
For a list of all the versions available, see the [tags][tags] and 
[releases][releases] on this repository. 

## Acknowledgements

Special thanks go out to the following people and projects who have helped in 
some way to make this project a reality.

* [@daniellmb/.github][daniellmb] - for the original idea to create a 
  `.github` template pack.
* [PurpleBooth/README-Template.md][purple-booth] - for the README file 
  inspiration.
* [Github][github-link] - for the `ISSUE_TEMPLATE` template files.


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

