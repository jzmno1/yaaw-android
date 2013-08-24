yaaw-android
============

YAAW packed into Android app using PhoneGap.

Yet Another Aria2 Web Frontend in pure HTML/CSS/Javascirpt.

Then packed into native mobile OS apps using PhoneGap. Faster and more convenient.

Currently only Android version available.

I'll be needing developer privilege for Windows Phone and iOS otherwise I can't make apps for them. And, sadly those are not free.

But I can provide iOS app signed with debug keys, if you want it, please open an issue and give me some time.

~~yaaw-android work with Aria2 1.41: https://www.box.com/s/h47cqmloqheuk1d5qysq~~

Try new Android version instead if you're running Aria2 1.61 or above.

WP7: https://www.box.com/s/7rp5fkhup4vdeimf6grx (debug key used)

Updated as YAAW pulled:

Be awared! Following versions do not support Aria2 1.41, might be OK if you're using 1.61 or above. New version includes new PhoneGap core and respond faster.

Android: https://github.com/jokies/yaaw-android

The newly released Aria2 1.71 worked like a charm, I recommend everybody reading this try it out immediately.

An already complied .apk file is included so you don't have to complie everything yourself. But I won't share my signing key, be awared, thanks.

<br />

Usage
-----
1. Run aria2 with RPC enabled
> aria2c --enable-rpc --rpc-listen-all=true --rpc-allow-origin-all -c -D
>
> Warning: This options will not verify the identity of caller. KEEP THE ADDRESS SECRET.

2. Open the program installed on your mobile device.

3. Change "JSON-RPC Path" setting if "Internal server error" occurred.

4. If login enabled, "JSON-RPC Path" must be like: "http://username:password@yourdomain.com:6800/jsonrpc"

5. Enjoy :-)

Tips
----
* All your settings on web is temporary. **Settings will be lost after aria2 restarted.**
* Tasks(including which is not finished) will be lost after aria2 restarted. Using `--save-session=SOME/WHERE` and reload with `--continue=true --input-file=SOME/WHERE` to continue.
* Using `$HOME/.aria2/aria2.conf` to save your options.
* For more infomations about aria2, visit [Aria2 Manual](http://aria2.sourceforge.net/manual/en/html/)

Components
----------
+ [Bootstrap](http://twitter.github.com/bootstrap/)
+ [mustache.js](https://github.com/janl/mustache.js)
+ [jQuery](http://jquery.com/)
+ [jQuery Storage](http://archive.plugins.jquery.com/project/html5Storage)
+ [JSON RPC 2.0 jQuery Plugin](https://github.com/datagraph/jquery-jsonrpc)
+ [PhoneGap 2.9.0](https://github.com/phonegap/phonegap)
+ [PhoneGap 2.9.0](https://github.com/phonegap/phonegap-plugins)

License
-------
yaaw and yaaw-android is licensed under GNU Lesser General Public License.
You may get a copy of the GNU Lesser General Public License from http://www.gnu.org/licenses/lgpl.txt
