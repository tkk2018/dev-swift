# @autoclosure

Allow to pass-in closure without mentioning open bracket `{` and close bracket `}`. This may make the code hard to read and understand.

One of the pratical usage is for logging purpose. Using closure can prevent the message being built if not required and using the `@autoclosure` can help the caller to keep the function simple. See [this example](https://stackoverflow.com/a/38335822/16027098).

## Limitation

The `@autoclosure` param is not allow to be `nil`. See [this for question for more info](https://forums.swift.org/t/optional-closure-with-autoclosure/10121
).
