# ESP-IDF tools and ressources

## .gitignore

```
build/
sdkconfig
sdkconfig.old
dependencies.lock
managed_components
pytest_embedded_log/
```

## build log colors

How to enable colors in build's log while doing ```idf.py build```:

```cmake
# To be added after "project" in the CMakeLists.txt
idf_build_set_property(COMPILE_OPTIONS "-Wno-error=class-memaccess" APPEND)
idf_build_set_property(COMPILE_OPTIONS "-fdiagnostics-color=always" APPEND)
```

