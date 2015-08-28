AOSPA Manifests
========================
Project for motorola Moto G 2014 LTE (THEA)

### Installing Repo ###
```bash
# Make a directory where Repo will be stored and add it to the path
    $mkdir ~/.bin
    $PATH=~/.bin:$PATH

# Download Repo itself
    $curl https://storage.googleapis.com/git-repo-downloads/repo > ~/.bin/repo

# Make Repo executable
    $chmod a+x ~/.bin/repo
```

### Initializing Repo ###
```bash
    $ repo init -u https://github.com/AOSPA/manifest -b lollipop-mr1

    $ curl --create-dirs -L -o .repo/local_manifests/localmanifest.xml -O -L https://raw.githubusercontent.com/RolanDroid/local_manifest/Lollipop-5.1.1/local_manifest.xml
```
### For sync: ###
```bash
    $repo sync -j4 (default)
    $repo sync -j32 (optional)
```
### and run the builder tool. ###
```bash
    $./rom-build.sh thea
```
