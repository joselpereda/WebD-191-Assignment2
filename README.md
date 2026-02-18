This demnos app uses the Fetch API to grab the RSS feed for my codepen profile. I've used a proxy (rss2json) to bypass the CORS restriction and turn the XML into a nice JavaScript object.

How it works:
Component	    Description
RSS Feed	    CodePen automatically generates a feed at codepen.io/joselperedca/public/feed/.
rss2json	    This is a free service that converts the XML feed into JSON. It also adds the necessary headers so your browser doesn't block the request (CORS).
Fetch API	    The fetch() function is the modern way to make AJAX calls. It's cleaner than the old XMLHttpRequest.
Async/Await	  This makes the code read linearly, even though the data fetching happens in the background.
