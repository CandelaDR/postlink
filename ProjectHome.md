# Description #
If a link is structured like:
```
<a href="http://yourserver.com/yourscript?option=value&option2=value">Link</a>
```
(which is a GET request to the server), postlink will convert the link to a temporary form so it can be a POST request to the script with the same query string.

# Usage #
```
<script type="text/javascript" src="jquery.postlink-0.1.js"></script>
<script type="text/javascript">
$(document).ready(function() {
  $('a').postlink();
});
</script>
```
# Benefits #
The benefit of using this plugin is that all requests to the server will be post requests instead of get requests.  This will also prevent the address bar from being "cluttered", especially applications that pass a session key with every request to the server.

---


_Note_:  This is my first attempt at creating a plugin for jQuery - I am hosting it with Google Code so I can hopefully get some input and help on making it better.