# PeterDB

This is the implementation of a relational database, also the project codebase for the class *Principles of Data Management*.

### Components

- PagedFileManager (pfm)
- RecordBasedFileManager (rbfm)
- RelationManager (rm)
- IndexManage (ix)
- QueryEngine (qe)

### Build

- `mkdir -p cmake-build-debug && cd cmake-build-debug`
- `cmake ../ && cmake --build .`

### Test

- `cd cmake-build-debug`
- `ctest .` or specify a test case, like `ctest . -R PFM_File_Test.create_file`

### Clean

- `rm -rf cmake-build-debug`