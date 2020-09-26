**Se**mantic **A**da

Ada libraries for the Semantic Web.


# Compiling
The requirements are

- the Ada GNAT compiler 
- the GPRBuild tools
- the [Matreshka library](https://forge.ada-ru.org/matreshka)

The usual sequence may work for your environment:

```
make
make install
```

The Makefile can be configure at the makefile.setup file. This file can be generated with the following command:

```
make setup
```

## With GPRBuild

Use the following commands to compile:

```
gprbuild -PSeA.gpr -p
```

To install the library and binaries:

```
gprinstall -PSeA.gpr -p
```

A install directory can be specified by the `--prefix` parameter:

```
gprinstall -PSeA.gpr --prefix=/home/USERNAME/Ada -p
```

# Usage
The API specification are available as `*.ads` files. 

Main programs were created for debuging purposes. They are `src/binaries/*.adb` source files and they are specified inside the `SeA_binaries.gpr` file at the `Main` variable.
These programs are used to test and debug the libraries. They can be used as examples.

# License
This work is under the General Public License version 3.
