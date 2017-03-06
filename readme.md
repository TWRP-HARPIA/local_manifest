LOCAL_MANIFEST
========================

### Installing Repo ###
```bash
# Make a directory where Repo will be stored and add it to the path
    $ mkdir ~/.bin
    $ PATH=~/.bin:$PATH

# Download Repo itself
    $ curl https://storage.googleapis.com/git-repo-downloads/repo > ~/.bin/repo

# Make Repo executable
    $ chmod a+x ~/.bin/repo
```

### Initializing Repo ###
```bash
    $ repo init -u git://github.com/omnirom/android.git -b android-7.1
    $ curl --create-dirs -L -o .repo/local_manifests/twrp.xml -O -L https://raw.githubusercontent.com/TWRP-HARPIA/local_manifest/twrp/twrp.xml
```
### For sync: ###
```bash
    $ repo sync -j4
```
### To build for your device.. ###
```bash
    $ source build/envsetup.sh
    $ breakfast harpia
    $ make -j5 recoveryimage
```


