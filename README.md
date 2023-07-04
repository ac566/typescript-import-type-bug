Steps:
1. `npm i` 
2. `npm test` or `tsc -P tsconfig.json`


Description:
* Actual: When importing only the type from another file, the entire file is included in the output
* Expected: Only files included directly in the tsconfig, or imported as values are included in the output

* Workaround: Setting "noResolve" to true, emits the correct output, but gives error during generation