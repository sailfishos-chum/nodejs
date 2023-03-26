# Node.js packaging for Sailfish OS

Based on the work of *b100dian*, Node.js packaging is following openSUSE
scripts and sources. Sources are stored directly at OBS together with
the SPEC file.

This repository contains [example SPEC](nodejs18.spec) that can be
used as a reference.

To update:

1. Checkout latest openSUSE sources from
   https://build.opensuse.org/package/show/openSUSE:Factory/nodejs18. One
   option is to use `osc`:
   ```
   `osc -A obs co openSUSE:Factory/nodejs18`
   ```
   with alias `obs` pointing to https://api.opensuse.org

2. In SailfishOS OBS repository copy, copy SPEC file somewhere for
   future use.

3. Copy all files except `_constraints` and into checked out
   SailfishOS OBS repository. Adjust openSUSE SPEC file to take into
   account all changes introduced into SPEC before. For that, use old
   copy of SailfishOS SPEC.


   