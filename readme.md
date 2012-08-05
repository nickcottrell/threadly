# Threadly
## Query string param detection

This needs to be refactored and redcued... but the bulk is there. Set the keyword and values to match in order to do something. The `DEBUG` var is configured for the parameter that occurs after an `&`. Hence, `http://url.com?keyword=value' will return as a match (if the values match) and `?keyword=value&debug` will also return as a match with a bunch of alerts.... i'm working on making this more clear with a few docs and a more some simpler script option that is much more stripped down.

### Demo
This one will do nothing:
http://istitch.net/threadly/demo.html

This one will return a successful match:
http://istitch.net/threadly/demo.html?needle=threaded

This one will return an unsuccessful value match
http://istitch.net/threadly/demo.html?needle=nope

This one will return an unsuccessful keyword match
http://istitch.net/threadly/demo.html?nope=threaded

This one will return a bunch of alerts wrapped in a debug conditional
http://istitch.net/threadly/demo.html?needle=threaded&debug

Same thing, but without a correct match
http://istitch.net/threadly/demo.html?needle=nope&debug
