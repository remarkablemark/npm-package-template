# npm-package-template

[![NPM](https://nodei.co/npm/npm-package-template.png)](https://nodei.co/npm/npm-package-template/)

[![NPM version](https://img.shields.io/npm/v/npm-package-template.svg)](https://www.npmjs.com/package/npm-package-template)
[![Build Status](https://travis-ci.org/remarkablemark/npm-package-template.svg?branch=master)](https://travis-ci.org/remarkablemark/npm-package-template)
[![Coverage Status](https://coveralls.io/repos/github/remarkablemark/npm-package-template/badge.svg?branch=master)](https://coveralls.io/github/remarkablemark/npm-package-template?branch=master)

npm package template.

## Installation

Clone repository with Git:

```sh
git clone https://github.com/remarkablemark/npm-package-template.git
cd npm-package-template
```

## Usage

Rename package (use [npm-package-name-checker](https://remarkablemark.org/npm-package-name-checker/) to check for name availability):

```sh
# replace $NAME with your package name
git grep -l npm-package-template | xargs sed -i '' -e "s/npm-package-template/$NAME/g"
```

Manually update the files:

- [ ] LICENSE
- [ ] README.md
- [ ] package.json

Reinitialize Git repository:

```sh
rm -rf .git
git init
```

Install package dependencies:

```sh
npm install
```

Make first commit:

```sh
git commit -am "feat: initial commit"
```

## Testing

Run tests:

```sh
npm test
```

Run tests in watch mode:

```sh
npm run test:watch
```

Run tests with coverage:

```sh
npm run test:coverage
```

View coverage in browser:

```sh
npm run test:coverage:report
open coverage/index.html
```

Lint files:

```sh
npm run lint
```

Fix lint errors:

```sh
npm run lint:fix
```

## Release

Only collaborators with credentials can release and publish:

```sh
npm run release
git push --follow-tags && npm publish
```

To see what files are going to be published, run the command:

```sh
npm pack --dry-run
# tar tvf $(npm pack)
```

## Support

- [Patreon](https://b.remarkabl.org/patreon)
- [Ko-fi](https://b.remarkabl.org/ko-fi)
- [Liberapay](https://b.remarkabl.org/liberapay)
- [Teepsring](https://b.remarkabl.org/teespring)

## License

[MIT](https://github.com/remarkablemark/npm-package-template/blob/master/LICENSE)
