LastFmApi
---------

A thin but dynamic wrapper around the Last.fm api webservice found at
http://ws.audioscrobbler.com/2.0/ - Currently, only unauthenticated endpoints
are supported. You are still required to provide an API key just not the
secret.

Installation is easy.

    pip install lastfmapi

Once that's done, you can do something as simple as...

    import lastfmapi
    
    api = lastfmapi.LastFmApi('<your api key here>')
    
    api.album_getInfo(artist='Cher', album='Believe')

For methods on the Last.fm api, simply call that method on the api object,
subsituting '_' where '.' would be.

* Unlike the master fork , this will require the requests library. *


Credit
---------

All of the credit of this goes to the original author this
was forked from. I only changed a few things in order to have
this lib work on python3+