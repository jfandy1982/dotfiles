# Andreas' dotfiles

I have started to implement scripts for my daily work with the private environments on various infrastructures like Windows or Linux etc. There are parts for regular operations like backing up data or extend the logon procedure by mounting shared network drives. Other parts are only relevant to bootstrap a new desktop environment or a virtualization environment.

I have also reviewed the tons of other dotfiles repositories, which are a great inspiration for this repository here. I will list the most important repositories at the end of this [README](#thanks) file.

As mentioned in almost every others' dotfiles repository, the functionality provided there might not work on every machine out of the box. This is also true for my repository, therefore the disclaimer is following.

**Disclaimer:** _The implementations are fitting to my personal needs. Other potential implementations are great as well. But these alternatives are not necessarily included here, if not really required for my personal needs. If you find these implementations useful anyhow, you may use them AT YOUR OWN RISK._

_Remark:_ I am not a user of any MacOS system. There are tons of dotfiles repos outside there focussing on that infrastructure.

## Private Files

I store private information in a second repository `dotfiles-private`. The configurations stored there are used in several scripts of this repository. For many cases, the private configuration is optional and not required at all. Scripts will have specific command-line options to include additional configuration from such a private repository, if necessary. Required configuration files are mentioned explicitly.

Example data stored in the private files:

- API keys
- private network configuration

## Installation

To initialize the dotfiles on the local environment, I have created [this Gist snippet](https://gist.github.com/jfandy1982/f2f0aadd010ff21a6b35c57e62bf6730). The script creates the required folders in the `${HOME}` directory of the current user, generates an SSH key for accessing GitHub and finally clones the required repositories. The repositories and the settings are hard-coded in the script up to now and can't be replaced.

Execute the following command to download the temporary script.

```bash
curl -SL https://gist.githubusercontent.com/jfandy1982/f2f0aadd010ff21a6b35c57e62bf6730/raw/e038fc2cebc8f57db86d89d92c2f5356b05f007b/clone_dotfiles_ubuntu.sh | bash
```

## Customization

You may check the various configuration files, which are stored in this repository. It should be possible to play around with the configurations in your local environment. Possible configurations for the initial setup are described in the specific section with a separate README.md file.

A few configurations might need your **attention**.

## Contributing

Please check out the [CONTRIBUTING.md](https://github.com/jfandy1982/.github/blob/main/CONTRIBUTING.md).

## Thanks

I would like to thank all those brave people, who have groomed the path to such a dotfiles repository. All the tons of such repos are a good inspiration - be it a functional or a structural inspiration. The ideas are worth to be checked.

A few repos are obviously the main starting point for many people - also for me. I would like to mention them here explicitly.

- [dotfiles@natelandau](https://github.com/natelandau/dotfiles)
- [dotfiles@mathiasbynens](https://github.com/mathiasbynens/dotfiles)
- [dotfiles@rkalis](https://github.com/rkalis/dotfiles)
- [dotMan@Bhupesh-V](https://github.com/Bhupesh-V/dotman)

Finally, [this curated list](https://dotfiles.github.io/) of dotfile projects, reports and links helps a lot to create a own project or repository.
