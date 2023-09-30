# PeterDB

This is an implementation of a relational database.

### Components

- PagedFileManager (pfm)
- RecordBasedFileManager (rbfm)
- RelationManager (rm)
- IndexManage (ix)
- QueryEngine (qe)

### Build

    rm -rf cmake-build-debug    # clear previous builds if exists
    mkdir -p cmake-build-debug  # create a sub-directory
    cd cmake-build-debug && cmake ../ && cmake --build .    # build with cmake

### Test

    cd cmake-build-debug
    ctest . # test all components
    ctest . -R PFM_File_Test.create_file    # test a specific function