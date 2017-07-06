# NativeScript Build Helper

[![npm version](https://badge.fury.io/js/%40holisticon%2Fnativescript-buildhelper.svg)](https://badge.fury.io/js/%40holisticon%2Fnativescript-buildhelper)
[![Issue Count](https://codeclimate.com/github/holisticon/nativescript-buildhelper/badges/issue_count.svg)](https://codeclimate.com/github/holisticon/nativescript-buildhelper) 
[![Dependency Status](https://david-dm.org/holisticon/nativescript-buildhelper.svg)](https://david-dm.org/holisticon/nativescript-buildhelper) 
[![devDependency Status](https://david-dm.org/holisticon/nativescript-buildhelper/dev-status.svg)](https://david-dm.org/holisticon/nativescript-buildhelper#info=devDependencies)

Basic NPM package for helping on automate releasing of NativeScript Apps

** CURRENTLY A PRE-RELEASE **

## Requirements

* Node 4+
* NativeScript 2.5+
* Git versioning system
* fastlane (if automatic upload is need)

## Installation

```
npm install @holisticon/nativescript-buildhelper --save-dev
```

Or if you want to use the development version (nightly build), which maybe not stable!:

```
npm install @holisticon/nativescript-buildhelper@next --save-dev
```

## Usage

For those who haven't deployed any apps in v2.4 of NativeScript; one of the new features that is turned on by default is SnapShots.    Now most the time this is a AWESOME thing, however occasionally this can cause issues.   For example I have one app of mine that this crashes at startup when using SnapShots.

Now the docs do list how to disable snapshots; but it is a lot easier for me to find the notes on my own site than trying to figure out which doc has the info.

The environmental variable you need to adjust is: <strong>TNS_ANDROID_SNAPSHOT</strong>

0 = Force Snapshots off always
1 = Force snapshots on (including in debug mode)
Unset = Snapshots only in Release mode
