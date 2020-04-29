# labscript-suite-bitbucket-archive
The labscript suite was originally hosted on BitBucket. 
With BitBucket dropping support for mercurial repositories, we were forced to migrate to git.
As Atlassian chose not to provide a mechanism to preserve repository metadata such as issues, pull requests, and commit comments, we moved to the industry standard git host (GitHub).
This repository hosts our attempt at preserving the repository metadata, that otherwise would be lost when Atlassian delete all hosted mercurial repositories.

This repository was generated using the [bitbucket-hg-exporter](https://github.com/philipstarkey/bitbucket-hg-exporter) tool created by labscript suite developer [Philip Starkey](https://github.com/philipstarkey).
The tool recursively downloads all BitBucket API data, saving each API endpoint as a JSON file.
We have done this for every public labscript-suite repository on BitBucket (including all forks).
A simple web frontend (written in AngularJS) is also contained within this repository so that the repository metadata can be viewed easily, and hosted using GitHub pages.

The result is a website that reasonably reflects the state of labscript suite repositories on BitBucket just prior to the migration to GitHub.
Links, commit hashes, etc, have been rewritten to point to the relevant page in this archive.
The actual code is also available on GitHub for [labscript suite](https://github.com/labscript-suite) repositories and all [forks](https://github.com/labscript-suite-bitbucket-archive).
BitBucket diff URLs contained in archived comments are rewritten as best we can to point to diffs on GitHub.

Issues have also been imported directly to GitHub repositories with commit hashes rewritten to match the relevant git commit.
We also reformatted issue links to point to both intra and inter-repository issues, and we provide an additional link to the version archived here too.
Links to pull requests have been rewritten to point to this archive.

We hope that this sufficiently archives the development discussions and history of the labscript suite.

The archive is visible here: [http://bitbucket-archive.labscriptsuite.org/](http://bitbucket-archive.labscriptsuite.org/).

## What to do if you think something is missing
There is a good chance that the missing information is contained within either the JSON files in this repository or migrated GitHub repositories.
The web front end does not display everything in the JSON files (mainly due to a lack of time).
We welcome pull requests that improve the web front end to display missing data.
Ideally these would be made to the [bitbucket-hg-exporter](https://github.com/philipstarkey/bitbucket-hg-exporter) project where the AngularJS template originated.

Should you find something missing prior to 30th June 2020, please let us know so we can save it from the BitBucket repositories!
Otherwise we expect that data to be unrecoverable as Atlassian have indicated every mercurial repository on BitBucket will be unceremoniously deleted after that date.
