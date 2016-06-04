I believe this should replace the current app on the app store "TCP Bulbs (connect)" as it's a more reliable integration.  

I did a couple of things to make this more reliable:
1.  I re-fetch the authorization token every 5 minutes
2.  If a request fails, I again re-try to fetch the token and re-submit the request
3.  I try again on 400 errors in addition to 500 and 401 errors.

Code is all open source under Apache 2.0 license. 
