# Purpose
Reads a pattern from the clipboard and tries to find a matching password in the given suffix with pass and types it. Feedback is given via libnotiy.

The advantage is that it is independant from the application you need the password for.

# Example usage

First I select the url base and then press:
* `Windows + P` for just the password.
* `Windows + Ü` for login and password.

This is an excerpt from `~/.xbindkeysrc`:
```
# password helpers
# type login information with pass
"pass-type-login.sh --login-first"
    m:0x40 + c:34

# type password information with pass
"pass-type-login.sh"
    m:0x40 + c:33
```

There is probably room for improvement but for now it works fine for me.

# Improvement

* Somehow read pattern or url from active window
* Browse multiple suffixes
* Allow different structure
