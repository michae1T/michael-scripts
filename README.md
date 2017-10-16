# michael-scripts

Some useful standalone scripts for improving console productivity split out from
[michael-bootstrap][1].

### vif ###

Simple wrapper combining vi with find -name or git status and git show.  Also optionally
supports the vim [file-line plugin][2].

Usage:

$ vif PATTERN[:LINE_NUM]

If there is more than one match a list of matches will be printed to the console
and the user can select the desired option by entering its number.  If there
is one match it will be opened automatically.  Line number will be applied to the
selected file.

$ vif -g [TAG]

If git tag or hash is included it will present selection for the files touched
in the changeset otherwise it will use git status.  file-line is not supported
in this mode.

It will also recognise and strip the a/ and b/ from the beggining of diff paths
to minimise keystrokes when working with git.

[1]: https://github.com/michae1T/michael-bootstrap
[2]: https://github.com/bogado/file-line.git
