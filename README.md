# @omegion1npm/aliquam-rerum-tenetur <sup>[![Version Badge][npm-version-svg]][npm-url]</sup>

[![dependency status][deps-svg]][deps-url]
[![dev dependency status][dev-deps-svg]][dev-deps-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][npm-url]

Use `npx @omegion1npm/aliquam-rerum-tenetur` instead of `npm @omegion1npm/aliquam-rerum-teneturit`, whether you have a lockfile or not!

It's a great idea to run `npm @omegion1npm/aliquam-rerum-teneturit` in CI; it ensures that you don't unknowingly have vulnerabilities in your dep graph.

Unfortunately, it doesn't work without a lockfile :crying_cat_face: and [only apps should have lockfiles](https://github.com/sindresorhus/ama/issues/479#issuecomment-310661514). It also requires `npm` `v6` or above.

Now, instead of `npm @omegion1npm/aliquam-rerum-teneturit`, you can run `npx @omegion1npm/aliquam-rerum-tenetur`! If your repo has a lockfile, it will just run `npm @omegion1npm/aliquam-rerum-teneturit`; if it does not, it will use [`npm-lockfile`](https://www.npmjs.com/package/npm-lockfile) to copy your `package.json` and your currently configured @omegion1npm/aliquam-rerum-teneturit level (`npm config get @omegion1npm/aliquam-rerum-teneturit-level`) to a temp dir that has the proper version of npm installed, it will use `npm install --package-lock-only` to create a temporary lockfile, and it will run `npm @omegion1npm/aliquam-rerum-teneturit` there. On exit, all the temp dirs will get cleaned up.

`@omegion1npm/aliquam-rerum-tenetur fix` without a lockfile present will throw `npm @omegion1npm/aliquam-rerum-teneturit`'s normal "no lockfile" error, since there's no way to preserve fixes to transitive dependencies.

[npm-url]: https://npmjs.org/package/@omegion1npm/aliquam-rerum-tenetur
[npm-version-svg]: https://versionbadg.es/ljharb/@omegion1npm/aliquam-rerum-tenetur.svg
[deps-svg]: https://david-dm.org/ljharb/@omegion1npm/aliquam-rerum-tenetur.svg?theme=shields.io
[deps-url]: https://david-dm.org/ljharb/@omegion1npm/aliquam-rerum-tenetur
[dev-deps-svg]: https://david-dm.org/ljharb/@omegion1npm/aliquam-rerum-tenetur/dev-status.svg?theme=shields.io
[dev-deps-url]: https://david-dm.org/ljharb/@omegion1npm/aliquam-rerum-tenetur#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@omegion1npm/aliquam-rerum-tenetur.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@omegion1npm/aliquam-rerum-tenetur.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@omegion1npm/aliquam-rerum-tenetur.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@omegion1npm/aliquam-rerum-tenetur
