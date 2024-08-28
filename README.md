# Reproduction of License Webpack Plugin not Emitting

1. Run `npm install`
2. Run `npx nx build app3`

Note that `3rdpartylicenses.txt` is not emitted.

3. Remove `overrides` from `package.json` (@nx/rspack will revert to using v0.7.5)
4. Run `npm install`
5. Run `npx nx build app3` 

Note that `3rdpartylicenses.txt` is emitted.
