# Success

Wooo! The server was able to verify you and stored your steam information!

FYI, registering another time will refresh your information in the database, and cause you to redo the next steps.

### What's next? 

To actually enable the server to recognize what calls are sent by you, a specific file must be present in the mod location. the next steps are described in detail in `#resources` on our discord server, so if that's how you came here, go back there.

To summarize, use the Discorsa bot to run the command `/discorsa get_toml`, take the file you get in return and put it in the Discorsa mod folder. Install the mod using content manager if you haven't already.

Confused?

[![Server Button]][Server Link]

[Server Link]: https://discord.gg/DPTCrxawBx
[Server Button]: https://img.shields.io/badge/Join_support_server-5865F2?style=for-the-badge


var docURL = window.location.href,
  params = [];

// filter out the website origin "example.github.io" in the OP example      
docURL = docURL.replace(window.location.origin, '');

// if /#/ found then we have URL parameters
// grabbing the parameters part of the URL
if (docURL.indexOf('/#/') > -1) {
  docURL = docURL.split('/#/')[1];
  if (docURL != '') {

    // omit the last forward slash if exist
    if (docURL[docURL.length - 1] == '/') {
      docURL = docURL.substring(0, docURL.length - 1);
    }

    // split the URL final string o get an object with all params 
    params = docURL.split('/');
    console.log(params);
  }
} else {
  console.log('No URL parameters found');
}
