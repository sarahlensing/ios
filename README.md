# The Mapzen iOS SDK

The Mapzen iOS SDK is a thin wrapper that packages up everything you need to use Mapzen services in your iOS applications.

We're currently under heavy development with this SDK. We welcome feature requests by posting an issue and labeling it appropriately as a "Feature Request". Feel free to also reach out to us using any of the other channels we have available on https://mapzen.com/

## Usage

At Mapzen we're developing our various SDKs using Xcode 8 and Swift 2.3. However, minor changes are needed to run in Xcode 7 / Swift 2.2. If you need Swift 2.2 support, or you run into any other issues, please open an issue ticket on Github and we'll figure it out together! 

The Mapzen iOS SDK uses Cocoapods to handle importing the various necessary dependencies that underpin our services. The full instructions for installing Cocoapods can be found on https://cocoapods.org/. As of the writing of this document, the Cocoapods installation instructions are diverged as Xcode 8's introduction has made backwards support of Xcode 7 challenging for the Cocoapods maintainers.

When you have installed the appropriate version of Cocoapods for your current development environment, run `pod install` from the command line inside the directory where you cloned this repository. Once that process completely (it can take several minutes depending upon how busy the github servers are that server Cocoapods), go ahead and open the `ios-sdk.workspace` file container to open the demo application codebase. 

## Notes

As noted above, we're currently under heavy development of this SDK. There's a couple of things you should probably know about up front:
* Right now due to an upstream dependency, we can currently only compile against iOS device targets. Keep an eye on this issue https://github.com/mapzen/ios/issues/32 as we add simulator support into our map renderer, Tangram-es, and then subsequently into the iOS SDK.
* Objective-C support is untested at this time, but will be happening in the near future - see this issue https://github.com/mapzen/ios/issues/68. If you run into issues in your obj-c project, feel free to comment on that issue.
