### pkg2deps
Validates if (a specific version of) Garden Linux can fulfill the package dependencies from an external package in a remote repository.

**Options**:
| Option | Example | Descriptions |
|--|--|---|
| -r (--repository) | http://ftp.debian.org/debian | Foreign/remote repository where the new package is located |
| -d (--dist) | trixie | The distribution to use within the remote repository |
| -p (--package) | dpkg | The name of the remote package within the remote repository |
| -v (--version) | 1.22.0 | The version of the remote package within the remote repository |
| -g (--gardenlinux-version) | 934.10 | The Garden Linux version to validate the package dependencies |
| -m (--missing) | NA | Also print completely missing packages |

**Usage**:

Example usage to evaluate if Garden Linux `934.10` can fulfill all package dependencies of the package `dpkg` in Debian `trixie` which is locate on the foreign/remote repository `http://ftp.debian.org/debian`.
```
./pkg2deps -r http://ftp.debian.org/debian -d trixie -v 1.22.0 -g 934.10 -p dpkg
```
