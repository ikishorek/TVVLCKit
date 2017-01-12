# VLCKit

VLCKit is a generic library for any audio or video playback needs on OS X, iOS and tvOS. It also supports active streaming and media to file conversations on the Mac. It is open-source software licensed under LGPLv2.1 or later, available in source code and binary form from the [VideoLAN website]. You can also integrate MobileVLCKit easily via [CocoaPods].

## Compile a new version

1. `./buildMobileVLCKit.sh -fb`. If building for tvOS, add `t` to the parameters (will be `-tfb`).
2. Update the `TVVLCKit.podspec` updating the version and linking it to the new framework version.
3. Replace the binary located in **build/TVVLCKit-binary** with the newer one located at **build/TVVLCKit.framework**.
4. Zip the TVVLCKit-binary folder and rename it "TVVLCKit".
5. Push changes to github and create a new release on [GitHub](https://github.com/PopcornTimeTV/TVVLCKit/releases), uploading the zipped TVVLCKit-binary folder as a binary.
