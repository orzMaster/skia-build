# Automated Skia builds for VS2019

This repo is forked from JetBrains/skia-build and dedicated to building Skia binaries for pure VS2019 project.

## Prebuilt binaries

Prebuilt binaries can be found [in releases](https://github.com/532479301/skia-build/releases).

## Why not use the binaries from JetBrains/skia-build

The Windows binaries from JetBrains/skia-build has two issues:
* The Debug version do not linked to VC's Debug runtime, but Release runtime. So any project linked to skia.lib count error when build debug version.
* Both binaries use VC's static Release runtime
