#minigrep

This is a command line program that implements the `minigrep` project from the [Rust book](https://doc.rust-lang.org/book/ch12-00-an-io-project.html).

Functionality:
- [x] Parse text files into lines
- [x] Find and print lines that contain the `query` argument from command line
- [x] Supports case-insensitive search via environment variable

## Running this program

You can run unit tests on this via:

`cargo test`

You can run the program via the following syntax:

`cargo run [query text] [text file]`

For example,

`cargo run frog poem.txt`

Note that poem.txt is included in this project.

##Case-insensitive Search

If you're using [PowerShell](https://docs.microsoft.com/en-us/powershell/), you can use the environment variable via the following:

`PS> $Env:CASE_INSENSITIVE=1; cargo run [query text] [text file]`

Since the variable will persist for the remainder of the shell session, you can unset it via the following:

`PS> Remove-Item Env:CASE_INSENSITIVE`
