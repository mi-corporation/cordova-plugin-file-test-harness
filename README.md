# Cordova Plugin File Test Harness

A harness for testing cordova-plugin-file during development.

cordova-plugin-file includes a Jasmine test suite packaged as a standalone Cordova plugin called cordova-plugin-file-tests. But you still need to provide a Cordova app that depends on that plugin, provides a copy of Jasmine, and registers the cordova-plugin-file-tests suite. This is a harness that does just that.

### How to use

1. Clone repo
1. Add cordova platforms as needed
1. To test local copies of cordova-plugin-file:
   ```
   > cordova plugin rm cordova-plugin-file
   > cordova plugin rm cordova-plugin-file-tests
   > cordova plugin add ./path/to/cordova-plugin-file
   > cordova plugin add ./path/to/cordova-plugin-file/tests
   ```
1. Run
   ```
   > cordova run <platform>
   ```
