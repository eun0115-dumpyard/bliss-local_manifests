BlissROM for Samsung Galaxy A71
------------------------------------

Create directories
```bash
mkdir bliss
cd bliss
```

Init the base manifest

```bash
repo init -u https://github.com/BlissRoms/stable_releases.git -b refs/tags/v17.8.2-universe --git-lfs --depth=1
cd .repo 
git clone https://github.com/eun0115-dumpyard/bliss-local_manifests local_manifests
cd ..
```

Then sync up with this command:
```bash
repo sync -c --force-sync --no-tags --no-clone-bundle -j4 --optimized-fetch --prune
```
-------------

_Building from source_
---------------
```bash
 . build/envsetup.sh
 blissify -g a71_userdebug
```
