# Monkey Wrench Content

1. Automatically calculate turbulence properties
* Use inline calculations to compute turbulence properties automatically.
* Also an example how to use substitutions and patchGroups to compact boundary
files
* Example case: tutorials/incompressible/pimpleFoam/pitzDaily
* Disclaimer: This is nothing new, just some useful things that are available
in OpenFOAM, collected in one tutorial for efficient case set-up.

2. Mesh narrow slots using snappyHexMesh
* A basic example of two narrow slots close to one another, meshed using
snappyHexMesh. Sometimes planar surfaces or narrow slots tend to be
castallated and not properly snapped. This case shows an example of
how to do this.
* Example case: tutorials/incompressible/simpleFoam/inclinedSlots

3. Mass zip/unzip files
* Zipping stl or obj files in a repo is usually a good idea, but sometimes you
need to be able to see the surfaces in ParaView. ParaView does not like zipped
files, so to make things faster here are two scripts to quicly unzip and re-zip
a bunch of files.
* Location: bin/gzipAll and bin/gunzipAll

4. Convert surface file mm to m scale
* OpenFOAM's surfaceTransformPoints utility can scale triangulated surfaces. Not
to retype the same syntax over and over again, here is a script that uses
surfaceTransformPoints to scale a geometry from mm units to m units for use with
snappyHexMesh.
* Location: bin/surfaceScaleMilimeterToMeter