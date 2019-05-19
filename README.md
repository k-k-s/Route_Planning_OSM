# Route Planning Project
Plans a route from point to point given by user on an Open Street Map using AStarSearch.
## Cloning

When cloning this project, be sure to use the `--recurse-submodules` flag. Using HTTPS:
```
git clone https://github.com/k-k-s/Route_Planning_OSM.git --recurse-submodules
```
or with SSH:
```
git clone git@github.com:k-k-s/Route_Planning_OSM.git --recurse-submodules
```

## Compiling and Running

### Compiling
To compile the project, first, create a `build` directory and change to that directory:
```
mkdir build && cd build
```
From within the `build` directory, then run `cmake` and `make` as follows:
```
cmake ..
make
```
### Running
The executables will be placed in the `bin` directory. From within `build`, you can run the project as follows:
```
../bin/<name-of-parent-directory> -f ../map.osm
```

## Testing

For exercises that have unit tests, the project must be built with the approprate test cpp file. This can be done by passing a string with the `-DTESTING` flag in `cmake`. For example, from the build directory:
```
cmake -DTESTING="Function Name" ..
make
```
Those commands will build the code with the tests for a specific function. The tests can then be run from the `build` directory as follows:
```
../bin/test
```
