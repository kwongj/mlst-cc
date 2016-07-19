# mlst-cc
Identifies similar MLST profiles from the same clonal complex

##Author

Jason Kwong (@kwongjc)

##Usage

```
$ mlst-cc -h
usage: 
  mlst-cc [profile] > clonal-complexes.txt

Identifies clonal complexes (CC) based on shared MLST alleles

positional arguments:
  profile          Tab-separated file with MLST alleles

optional arguments:
  -h, --help       show this help message and exit
  --shared shared  Number of shared MLST alleles to define clonal complex
                   (default = 6)
  --version        show program's version number and exit
```

##Bugs

Please submit via the [GitHub issues page](https://github.com/kwongj/mlst-cc/issues).

##Software Licence

[GPLv3](https://github.com/kwongj/mlst-cc/blob/master/LICENSE)
