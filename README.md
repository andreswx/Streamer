**************
Streamer - .Net / Unity access to the Twitter Streaming API

by Eddie Cameron (@eddiecameron / www.grapefruitgames.com)
**************

A simple API to let your .Net or Unity apps access the deluge of information available on the live Twitter stream.
Simplify connection, JSON parsing and OAuth handling.

**************
To use:
- create a new TwitterAccess object
- Either fill out OAuth application/access tokens, or provide user/password with BasicAuthUserPassword()
- Add at least one query parameter with AddQueryParameter()
- Call Connect()
- As tweets come in, they will be parsed and placed in the "tweets" queue

- see the example main.cs or go to http://grapefruitgames.com/2012/02/25/streamer-net-unity-access-to-the-twitter-streaming-api/ for more info

************** 

v0.9 - Initial public release
- Set up location and track query parameters on the /filter method (streaming only)
- Has basic auth, or, if you set up your own access tokens, OAuth
- Parses status, username, location and hashtags from the live feed. May ignore tweets with unusual characters in the status.

**************

TODO:
- add more query options
- support for getting user tokens from OAuth
- this will open up possibility for Twitter REST API access (post tweets, access a users timeline, etc)
- places support (currently only supports coordinates)