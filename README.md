# NodeJS Addon cpp

* npm i node-gyp node-addon-api

node-gyp configure  
node-gyp build  

## without node-gyp compile on OSX
```
gcc -undefined dynamic_lookup \
-mmacosx-version-min=10.7 \
-arch x86_64 \
-stdlib=libc++ \
-std=gnu++1y \
-I ~/Documents/src/nodejs/node-v10.15.3-darwin-x64/include/ -o test.node test.cc
```
