Twitter
=======

Stream tweets from the web

This script is to understand how to extract tweets near real time based on selected hashtags

Information on extraction from many sources as explained below
* https://dev.twitter.com/discussions/3449

curl -d @words https://stream.twitter.com/1/statuses/filter.json -uUSERNAME:PASSWORD

where words is a text file of the format:

track=stuff

Where stuff is the hashtag you want to follow. 
* Information from @ngramsky

---
* http://stackoverflow.com/questions/14298539/live-streaming-tweets-without-being-rate-limited

You can do live processing on twitter through Twitter Stream API. But stream api doesn't send you all tweets, you have to specify either keywords to filter tweets containing given keywords or userIds to follow tweets coming from given users or geo location to filter tweets coming from a particular place. Also there are limits on number of keywords, user ids to follow etc. And lastly twitter will give you upmost 1% percent of the tweets in the global traffic. So for example if you come up with a filter which tracks less than 1% of the global trafic you will get all the tweets (in theory) otherwise you will miss some tweet as twitter won't share them with you. 
* Information from stackoverflow.com
* More info at https://dev.twitter.com/docs/api/1.1/get/statuses/sample
* ...and https://dev.twitter.com/docs/streaming-apis/streams/public


