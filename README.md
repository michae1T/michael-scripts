# michael-scripts

Some useful standalone scripts for improving console productivity split out from
[michael-bootstrap][1].

### vif ###

Simple wrapper combining vi with find -name.  Also optionally supports the vim
[file-line plugin][2].

Usage:

$ vif PATTERN[:LINE_NUM]

If there is more than one match a list of matches will be printed to the console
and the user can select the desired option by entering it's number.  If there
is one match it will be opened automatically.  Line number will be applied to the
selected file.

It will also recognise and strip the a/ and b/ from the beggining of diff paths
to minimise keystrokes when working with git.

[1]: https://github.com/michae1T/michael-bootstrap
[2]: https://github.com/bogado/file-line.git
