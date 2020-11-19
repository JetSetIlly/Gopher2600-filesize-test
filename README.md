# Gopher2600-filesize-test

Two versions of Gopher2600 one commit apart. Comparing three version of the go
compilers (all linux/amd64). All sizes in bytes and are unstripped.

In all instances the build command is:

	> go build .


The version tagged `old` compiles to a relatively small binary.

| Go     | FileSize |
|:------:|:--------:|
| 1.13.6 | 15123696 |
| 1.14.6 | 15019728 |
| 1.15.5 | 14091976 |


The version tagged `new` compiles to a relatively large binary.

| Go     | FileSize |
|:------:|:--------:|
| 1.13.6 | 80394048 |
| 1.14.6 | 89182400 |
| 1.15.5 | 48805880 |


Stripped versions of all binaries are consistently around 5MB smaller in all
instances and have not been included here.



Parent project here: https://github.com/JetSetIlly/Gopher2600

