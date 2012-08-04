# Threadly
## Query string param detection

This needs to be refactored and redcued... but the bulk is there. Set the keyword and valid matches. The `DEBUG` var is configured for the parameter that occurs after an `&`. Hence, `http://url.com?keyword=value' will return as a match (if the values match) and `?keyword=value&debug` will also return as a match with a bunch of alerts.... i'm working on making this more clear with a few docs and a more some simpler script option that is much more stripped down.
