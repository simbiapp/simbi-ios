# Building Guide

## Prerequisites
 * OS X 10.9.4 (Mavericks)
 * Xcode 6

If you don't have Xcode, you can download it for free on the Mac App Store.

You can skip any step in this guide if you already have the required tools installed.

## Steps
### 1. Install homebrew
[Homebrew](http://brew.sh/) is a command line utility that makes it very easy to download and install more programs.  To install homebrew, run the following command in Terminal:
```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
Now update homebrew's list of packages with this command:
```
brew update && brew upgrade
```
### 2. Install git
Now that you've installed homebrew, you can use it to install packages like.  Installing things with homebrew is easy, just run this command:
```
brew install git
```
### 3. Install RubyGems
RubyGems is a package manager we will use to install cocoapods (which manages the dependencies for our project).  We will install it with git. 
```
git clone https://github.com/rubygems/rubygems.git
cd rubygems
sudo ruby setup.rb
```
### 4. Install cocoapods
Now, we will use RubyGems to install cocoapods.
```
gem install cocoapods
```
### 4. Clone the git repository
Navigate to the directory you want to put the project in using `cd`.  Then, clone the git repo using:
```
git clone https://github.com/simbiapp/simbi-ios.git
```
You may need to input your GitHub username and password when prompted.
### 5. Use cocoapods to install required dependencies
```
cd simbi-ios
cd simbi-app
pod install
```
### 6. Open the project in Xcode and build!
Now the project should be setup and install along with all of its dependencies.  Open the workspace file in Xcode using:
```
open simbi_app.xcworkspace
```

Tell us on [Slack](https://simbiapp.slack.com/messages/general/) if you have any issues.  Thanks for helping with the project!
