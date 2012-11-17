# My fork of the original [GENIA Tagger](http://www-tsujii.is.s.u-tokyo.ac.jp/GENIA/tagger/)

The main purpose of this repository is to serve as a reference for the [port to Java](https://github.com/jmcejuela/jeniatagger). The original source code (v 3.0.1) is found in the tag [original](https://github.com/jmcejuela/geniatagger/tree/original)

For info about the original program, see [original README](https://github.com/jmcejuela/geniatagger/blob/master/README)


## Few Improvements

* The original generated binary `geniatagger` can only be called from its same path as it makes static local references to some files. You can use the the simple bash script `apply-geniatagger` to overcome this.

## Known Issues

* The program has to load with every run some big dictionary files which can take quite a lot of time (~15s on a modern machine). The program should be rewritten to be more library-oriented and be able to keep the loaded dictionaries in memory. If you ron on the JVM, you can use the [Java port](https://github.com/jmcejuela/jeniatagger).
