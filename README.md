# yamlcheck

Check if files adhere to <a href="http://www.yaml.org/">YAML</a> syntax.

Quite simple and mostly useless.

* Version: 0.1.0
* Author: Felix Kaiser <felix.kaiser@fxkr.net>
* License: revised BSD (see LICENSE)


## Usage

```
positional arguments:
  PATHS

optional arguments:
  -h, --help     show this help message and exit
  -V, --version  show program's version number and exit
  -q, --quiet
```


## Demo

```
% ./yamlcheck samples/sample_correct.yml

% ./yamlcheck samples/sample_incorrect_*.yml
Error in samples/sample_incorrect_1.yml:3
  Context: line 3, column 1
    while parsing a flow node
  Problem: line 3, column 1
    expected the node content, but found '<stream end>'

Error in samples/sample_incorrect_2.yml:3
  Context: line 3, column 1
    while parsing a flow node
  Problem: line 3, column 1
    expected the node content, but found '<stream end>'
```

