---
title: iOS
date: 2016-09-29 15:27:11
layout: stack
---
iOS developers at Nodes build user-centric applications and extensions which are distributed on the App Store or through enterprise distribution platforms.

We deliver a range of applications for different platforms and devices like the iPhone, iPad, Apple Watch and Apple TV. 

### Tasks
 - Writing business and view logic with testability in mind
 - Setting up and maintaining unit and UI tests
 - Integrating with in-house or external APIs and services
 - Maintaining and setting up Apple services and applications 
 - Consulting with our UX team and clients to provide best possible product

## Stack

### Language

##### Swift
We've started with Swift as soon as version 1.0 was released and since then we have migrated all our projects through Swift 2 up to Swift 3 and we make sure all our frameworks and dependencies support all versions of the language.

##### Objective-C
Objective-C is a thing of the past for us, but occasionally we do maintain projects or update applications still written in Objective-C.

### Architecture

Clean architecture (known as VIPER when applied to iOS development) is our new standard on the iOS team. We also still maintain many apps that use MVC. Our clean architecture implementation is adapted to better fit our needs, with the goals being consistency, quality, and testability. 

### IDE
Xcode is the IDE that is widely used amongst iOS developers and we also use it at Nodes. 

### Other tools
 - [Carthage](https://github.com/Carthage/Carthage) - our weapon of choice for dependency management, simple yet powerful
 - [Model Boiler](https://github.com/nodes-ios/ModelBoiler) - a macOS application used to generate boilerplate code for model objects using Serializable
 - [Charles Proxy](https://www.charlesproxy.com/) - effectively serves as a MitM proxy which captures all network traffic and helps us debug network issues
 - [MacDown](http://macdown.uranusjr.com/) - for writing READMEs and blog posts like this one
 - [Zeplin](https://zeplin.io/) - makes it easy to transfer designs to code by providing exact measurements, colors and assets
 - [Postman](https://www.getpostman.com/) - all our APIs are documented through Postman allowing us to easily work together

### Libraries
These are the 3rd party libraries we usually use in all our projects. If there are other services required for a project, for example a Facebook Login, we also use their related SDKs.

 - [Alamofire](https://github.com/Alamofire/Alamofire) - an elegant HTTP networking library 
 - [Kingfisher](https://github.com/onevcat/Kingfisher) - a lightweight library for downloading and caching images from the web
 - [UrbanAirshipSDK](https://github.com/urbanairship/ios-library) - integrates with Urban Airship to register for and handle push notifications
 - [HockeySDK](https://github.com/bitstadium/HockeySDK-iOS) - integrates with HockeyApp to collect crash reports and show application updates during testing
 - [SnapKit](https://github.com/SnapKit/SnapKit) - a DSL to make Auto Layout easy
 - [netfox](https://github.com/kasketis/netfox) - one line setup network debugging library useful during QA process
 - [GoogleAnalytics](https://developers.google.com/analytics/devguides/collection/ios/v3/) - analytics and tracking library from Google
 - [Mixpanel](https://github.com/mixpanel/mixpanel-iphone) - advanced analytics and user tracking library with features like A/B testing and push notifications
 
### Open source
The iOS team at Nodes strives to deliver the best and nicest product and to allow us to do so, we've created many open source frameworks to make the development process faster, easier and safer. All of our repositories are maintained on [Github](https://github.com/nodes-ios/).

 - [Serpent](https://github.com/nodes-ios/Serpent) - fastest and most feature complete serialization library
 - [Blobfish](https://github.com/nodes-ios/Blobfish) - unified and abstracted visual handling of errors
 - [KeyboardHelper](https://github.com/nodes-ios/KeyboardHelper) - easy to use interface for handling keyboard events
 - [NStackSDK](https://github.com/nodes-ios/NStack) - integration with NStack for translations, version updates and more
 - [Cashier](https://github.com/nodes-ios/Cashier) - a simple, but effective 2-layer caching library suitable for most projects
 - [Noted](https://github.com/nodes-ios/Noted) - a more Swift-ier implementation of the observer pattern
 - [Codemine](https://github.com/nodes-ios/Codemine) - a collection of tweaks, utilities and nice-haves we use regularly
 - and many more...

### Continuous Integration

We have setup a continuous integration server using Bitrise.io, so that our builds, tests and deployments are easy, fast and consistent. Our Bitrise workflow uses Fastlane for building, signing, and uploading builds to both Hockey and Testflight. We also have some custom Ruby scripts for validation and reporting. 

