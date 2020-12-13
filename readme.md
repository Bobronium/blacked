# blacked
## [black](https://github.com/psf/black), but with single quotes
### What's wrong with other 'single-quoted' black options:
- [brunette](https://github.com/odwyersoftware/brunette): uses monkey patching that basically doesn't work when running against multiple files [odwyersoftware/brunette#5](https://github.com/odwyersoftware/brunette/issues/5)
- [axblack](https://gith️ub.com/axiros/axblack): forked from black a while ago, inconsistent with current black versions [axiros/axblack#7](https://github.com/axiros/axblack/issues/7)



### ToDo:
- add tests:
  - Both `blacked -S` and `black -S` must produce same results
  - `blacked` run against code formatted with `black` must change only quotes and vice-versa
  - `blacked` must adopt any currently installed `black` version
  - Tests must include running `blacked` against multiple files to assure multiprocessing works as expected
  - Tests must include latest or all `black` versions
- add support for config.cfg
- add support for blackd
