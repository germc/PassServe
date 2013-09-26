PassServe
=========

Two files that will make your life much easier. 

Requirements:
------------
AFNetworking - https://github.com/AFNetworking/AFNetworking

Compatibility
------------
Tested on iOS 7, might work on iOS 6

Installation
-----------
Unzip the archive and drag the files in the archive into your Xcode project.
Add: ```#import "PassServe.h"``` into the file which you will download passes with.

Usage
-----
To generate a pass on a remote server, use:

    [PassServe generatePassWithURL:@"http://pass.keatonburleson.com/example.php?name=%@" argument:@"joejoeboom" activityView:spinny webView:webView];

To download a pass from a remote server use:
     
    [PassServe downloadPassWithURL:[NSURL URLWithString:@"http://pass.keatonburleson.com/SavedPasses/pass.pkpass"] passName:@"joejoeboom.pkpass" webView:webView tableView:self.tableView overwrite:true];
     
Future Plans
------------

- ~~Download pass from remote source~~
- ~~Generate pass from remote source~~
-    Full logging mode
