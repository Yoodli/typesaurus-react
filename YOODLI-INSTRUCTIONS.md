* We are just doing this to fix some dependency errors.
* (so far) we've only changed package.json, and in unimportant ways.
* We will move off of this as soon as a working version is published.
* we could have done a github-hosted npm package, but seriously this should just be temporary.
* If you change anything:
```shell
cd typesaurus-react
npm i
# it has a fancy build process
make build
# clobber our existing copy
rm -r ../yoodli-client/typesaurus-react 
cp -r ./lib/reactopod ../yoodli-client/typesaurus-react
cd ../yoodli-client
# not sure if this is really needed:
npm i
```