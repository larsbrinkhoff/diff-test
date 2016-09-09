In the first revision, `foo` is a plain text file.  In the next
revision, I inserted a NUL, which makes git think it's a binary file.
But [adding the diff attribute](.gitattributes) makes git show the
diff anyway.  Try e.g. `git show 6e002f2`.

GitHub, however, does not show a diff:
https://github.com/larsbrinkhoff/diff-test/commit/6e002f286899972f6ff74b358c3327a6f7eb079d
