# mlst-cc
Identifies similar MLST profiles from the same clonal complex

## Author

Jason Kwong (@kwongjc)

## Requirements
* Python 3.x
* (not required, but recommended) [mlst](https://github.com/tseemann/mlst)

## Usage

```
$ mlst-cc -h
usage: 
  mlst-cc --scheme [scheme] > clonal-complexes.txt

Identifies clonal complexes (CC) based on shared MLST alleles

optional arguments:
  -h, --help       show this help message and exit
  --db db          Path to db (default = /home/tseemann/git/mlst/db/pubmlst)
  --scheme scheme  MLST scheme
  --list           List MLST schemes available
  --shared shared  Number of shared MLST alleles to define clonal complex
                   (default = 6)
  --version        show program's version number and exit
```

**For basic usage:**
```
mlst-cc --scheme kpneumoniae
```
where `--scheme` specifies the MLST scheme.

**To see which PubMLST schemes are supported:**
```
mlst-cc --list
```

**To change the location of the database directory:**
```
mlst-cc --db /path/to/dir
```
The database directory should contain a tab-separated file for each scheme containing the profiles for each defined sequence type. Highly recommended to use the database structure from Torsten Seemann's [MLST](https://github.com/tseemann/mlst) tool.


## Bugs

Please submit via the [GitHub issues page](https://github.com/kwongj/mlst-cc/issues).

## Software Licence

[GPLv3](https://github.com/kwongj/mlst-cc/blob/master/LICENSE)
