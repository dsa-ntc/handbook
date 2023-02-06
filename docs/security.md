# Security

## For our organization

We treat all information online as at risk of public exposure. This includes chat logs and communications on NTC infrastructure as well as the git histories of private repositories.

Report security concerns within the NTC to [ntc@dsacommittees.org](mailto:ntc@dsacommittees.org) and [techteam@dsausa.org](techteam.dsausa.org).

## For members and contributors

### Password Managers and Two Factor Authentication
The NTC requires unique, strong passwords for every service that you log into. For this reason, the NTC requires use of a password manager and recommends Bitwarden as it is currently the most full-featured open source password manager.

Use both a unique, strong password (or multi-word passphrase) and two-factor authentication (TFA or 2FA) where available to secure your password manager.

### Securing your identity in git commit logs

Some contributors choose to separate their political work from other spheres. When pushing work to a git host like Github or Gitlab there are two primary safeguards available: hiding your email address and using an entirely separate account. The latter (literally creating a second account with the hosting service) can be cumbersome, but a good choice if you want no connection between a public persona and your DSA-related work.

In addition, it's always a good idea to commit from a host-provided `noreply` email address. This limits exposure of your details to bots or other users who gain access to a repo. If you would like to commit using a different name or email address you can override the local git configuration from a repository. See more detailed documentation for [Github here](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/setting-your-commit-email-address).

```shell
# Within a dsa repository
$ git config user.name “Camille DSA”
$ git config user.email “69420-camille@users.noreply.gitlab.com”

# Now future commits will be tagged with
# Author: Camille DSA <69420-camille@users.noreply.gitlab.com>
```

Please note that merged code, including the git history, should be considered permanent. In the event a private repository is migrated to open-source the NTC should make an effort to contact past contributors, but as with all things online please approach your code contributions with these principles in mind (this includes things like commit messages, test data, and so on).


