# Access Control Matrix

Lay out the [access control matrix](https://en.wikipedia.org/wiki/Access_control_matrix) levels and some broad scope of what these do.




Access matrix for gitlab (no longer using this but moving this to this article for later reference):

* `Guest/Reporter` roles - More appropriate for my external-facing projects, Should be done per project just to keep the overall membership spread small.
* `Developer` - Default access for NTC mobilized members and collaborators who need to contribute to the repository. Should be the default group for projects as well. Developers _can_ edit project Wikis.
* `Maintainer` - NTC Project Stewards, NTC Department and Commission Leaders (Maybe not SC directly, Ian/John's role?), appropriate technical leads where present. Basically this should be seen as formal or informal leadership and has the final say for merging code, along with adding or removing contributors under this project or project group.
* `Owner` - Staff, NTC Leadership. Has power to delete projects. Should be treated with high security.