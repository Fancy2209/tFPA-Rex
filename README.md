Extract the game files from the GOD file into a folder called game in the root of the repository, then run the following:

For windows:
```
cmake --preset win-amd64 
cmake --build --preset win-amd64-debug --target tfpa_codegen
cmake --preset win-amd64 
cmake --build --preset win-amd64-debug
```

For linux:
```
cmake --preset linux-amd64 
cmake --build --preset linux-amd64-debug --target tfpa_codegen
cmake --preset linux-amd64 
cmake --build --preset linux-amd64-debug
```