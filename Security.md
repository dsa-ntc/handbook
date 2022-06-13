# Security

We treat all information online as at risk of public exposure. This includes chat logs and communications on NTC infrastructure as well as the git histories of private repositories.

## Securing your identity in the commit log

Some contributors choose to separate their political work from other spheres. If you would like to commit using a different name or email address you can override the local git configuration from a repository. Gitlab has instructions for setting up an anonymous account-specific email address [here](https://docs.gitlab.com/ee/user/profile/index.html#use-an-automatically-generated-private-commit-email). Github has a similar functionality.

```shell
# Within a dsa repository
$ git config user.name “Camille DSA”
$ git config user.email “69420-camille@users.noreply.gitlab.com”

# Now future commits will be tagged with
# Author: Camille DSA <69420-camille@users.noreply.gitlab.com>
```

Please note that merged code, including the git history, should be considered permanent. In the event a private repository is migrated to open-source the NTC should make an effort to contact past contributors, but as with all things online please approach your code contributions with these principles in mind (this includes things like commit messages, test data, and so on).

## Password Policy
Passwords are used to protect many of our systems and services.

Layout password policy here

## Password Managers and Two Factor Authentication
The NTC requires unique, strong passwords for every service that you log into. For this reason, the NTC requires use of a password manager and recommends Bitwarden as it is currently the most full-featured open source password manager.

Use both a unique, strong password (or multi-word passphrase) and two-factor authentication (TFA or 2FA) to secure your password manager.
