# chromeextension
chrome extension for easy link access 

. google chrome extenctions are created with these technologies HTML,CSS,JAVASCRIPT.
. Extension files are zipped into a  package of .crx extension that the user downloads and installs. 
. Extensions are distributed through the Chrome Developer Dashboard and published to the Chrome Web Store. 

        https://chrome.google.com/webstore/developer/dashboard
        https://chrome.google.com/webstore/category/extensions
        
        https://developer.chrome.com/webstore
        
.Take a small step into extensions with this quick simple Extensions example. Start by creating a new directory to store the extension's files

Next, add a file called manifest.json and include the following code:


{
  "name": "Quick link Extensions",
  "description" : "Base Level Extension",
  "version": "1.0",
  "browser_action": {
    "default_popup": "link.html",
    "default_icon": "icon.png"
  },
  "manifest_version": 2,
  "commands": {
    "_execute_browser_action": {
      "suggested_key": {
        "default": "Ctrl+Shift+Q",
        "mac": "MacCtrl+Shift+Q"
      },
      "description": "Opens quick link.html"
    }
  }
}


Every extension requires a manifest, though most extensions will not do much with just the manifest. For this quick start, the extension has a popup file and icon declared under the browser_action field:

Then create a file titled link.html:

{::nomarkdown}

 <!-- <html>
    <body>
      <h1>Qiick Link Extensions</h1>
    </body>
  </html>
  -->
{:/}



The Final step is to install the extension on your local system.


1) Navigate to chrome://extensions in your browser. You can also access this page by clicking on the Chrome menu on the top right side of the Omnibox, hovering over More Tools and selecting Extensions.
2) Check the box next to Developer Mode.
3) Click Load Unpacked Extension and select the directory for your "Quick Link Extensions" extension.

  ***  Now You can now use your popup-based extension by clicking the icon.png icon or by pressing Ctrl+Shift+Q on your keyboard. ****






























