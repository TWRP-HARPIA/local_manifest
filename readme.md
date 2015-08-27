AOSPA Manifests
========================
Project for motorola Moto G 2014 LTE (THEA)


Initializing Repo

    repo init -u https://github.com/AOSPA/manifest -b lollipop-mr1

    curl --create-dirs -L -o .repo/local_manifests/local_manifest.xml -O -L https://raw.github.com/RolanDroid/manifest/cm12.1/local_manifest.xml

For sync:

    repo sync -j4 (default)
    repo sync -j32 (optional)

and run the builder tool.

 ./rom-build.sh DEVICE
