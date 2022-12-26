# SwiftOS
AOSP ROM with Simplified Upgrade

### Requirements
- Around 500GB disk space.
- Around 18GB RAM running Linux OS.
- 2 or more CPU Cores

### Sync our source ###
```bash
        repo init -u https://github.com/SwiftAOSP/sw_manifest -b 13
        repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build our source ###
```bash
        . build/envsetup.sh
        lunch swift_$devicecodename-userdebug
        make sweet
```
