# Wildcard Match (WIP)

Wildcard Match provides an enhanced `fnmatch` and `glob` library. In some ways it is similar to Python's builtin `fnmatch` and `glob` as it provides functions to match, filter, and glob the file system. But it adds a number of features found in Bash's globbing such as backslash escaping, brace expansion, extended glob pattern groups, etc. It also adds a path centric matcher called `globmatch` which functions like `fnmatch` for paths. Paths that would normally be returned when providing `glob` a pattern should also be properly match in `globmatch`.

- Adds support for `**` in glob.
- Adds support for escaping characters with `\`.
- Adds support for brace expansion: `a{b,{c,d}}` --> `ab ac ad`.
- Adds support for extended match patterns: `@(...)`, `+(...)`, `*(...)`, `?(...)`, and `!(...)`.
- Adds ability to match path names via `globmatch` as well as traditional file system searching via glob.
- And more...

If all you are looking for is an alternative `fnmatch` and/or `glob`, Wildcard Match has you covered, but Wildcard Match also adds a file search utility called `wcmatch` that is built on top of `fnmatch` and `globmatch`. It was originally written for [Rummage](https://github.com/facelessuser/Rummage), but split out into this project to be used by other projects that may find it's approach useful.

## Documentation

http://facelessuser.github.io/wcmatch/

## License

The MIT License (MIT)

Copyright (c) 2018 Isaac Muse

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
