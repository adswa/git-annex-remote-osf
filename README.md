# OHBM BrainHack project: git-annex-remote-osf
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->
[![Documentation Status](https://readthedocs.org/projects/datalad-osf/badge/?version=latest)](http://docs.datalad.org/projects/osf/en/latest/?badge=latest)

Hey there :wave:

Welcome to our project. This repository is a place to develop a new [git-annex special remote](https://git-annex.branchable.com/special_remotes/) for the [Open Science Framework](https://osf.io/) data storage, and we will start doing so at the OHBM Brainhack 2020.

## Project description and aims

The [Open Science Framework (OSF)](https://osf.io/) is an amazing infrastructure for open science. In this project, we attempt to create a [git-annex special remote](https://git-annex.branchable.com/special_remotes/) implementation to leverage OSF filestorage and make the data storing that OSF provides even more useful. The git-annex OFS special remote would allow to transform OSF storage into git-annex repositories. Files in OSF storage could thus be consumed or exported fast and easily via git-annex or [datalad](https://github.com/datalad/datalad), and published to repository-hosting services (GitHub, GitLab, Bitbucket, ...) as lightweight repositories that constitute an alternative access to the data stored on the OSF - that is: you can ``git clone`` a repository from for example GitHub and ``get`` the data from the OSF from the command line or in your scripts.

During the Brainhack, we want to...
- Familiarize ourselves with git-annex's concept of special remotes
- Explore the [OSF API ](https://developer.osf.io/#tag/Introduction) and [OSF's waterbutler](https://github.com/CenterForOpenScience/waterbutler) to interact with OSF's various supported file storage services
- Get started with a Python-based special-remote implementation
- Short term goal: export and import data from public OSF projects from and into git-annex repositories
- Nice-to-have's/Long(er) term development goals: Extend functionality to private repositories (requires token-based authentication)

**EDIT**: Technical development takes place in https://github.com/datalad/datalad-osf as a DataLad extension, this repository is used for coordination. :+1:


## How can you help?

There are many ways in which you can help. If you haven't yet heard of git-annex or special-remotes, don't be discouraged. You can use or develop your skills in many other ways. Here are a few "good first issues":

- Set up the [allcontributors-bot](https://allcontributors.org/) in the project repository to acknowledge contributions
- Create a public and a private project on the Open Science Framework for us to play with. The more comprehensive this task is carried out, the better. Here's a sketch: Add (any) data (honestly, any - cat content, your favorite recipe, a funny video, ...) to different storage providers (OSFStorage, GDrive, Dropbox, ...) to a public and a private repository on the OSF. Make sure that some data exists in a single version, but also take data and update it with a modified version, using the [OSF's version control features](https://help.osf.io/hc/en-us/articles/360019738694-file-revisions-and-version-control).

Beyond these concrete actions, feel free to just join our discussions in this repository or via our communication channels. Here is a non-exhaustive list of skills that can be helpful:

- **Technical writing**: Good user documentation is essential. Depending on what you are interested to do this could take the form of a README, a [readthedocs](https://readthedocs.org/) or [Mkdocs](https://www.mkdocs.org/)-based technical documentation, tutorials, a usecase in the [DataLad handbook](http://handbook.datalad.org/en/latest/), or anything else that you can think of.
- **Experience with the Open Science Framework**: If you are a user of the Open Science Framework, let us know how you use it, walk us through a public project of yours, provide us with projects to use for testing, your ideas and needs,  ... If you have used the OSF then you will be a great help!
- **Python programming**: We aim for a special remote implementation in Python. There are [good templates](https://github.com/Lykos153/AnnexRemote) and [many](https://github.com/CONP-PCNO/git-annex-remote-globus) [examples](https://github.com/Lykos153/git-annex-remote-googledrive) that we will use and learn from along the way.
- **Interest in git-annex or experience with it**: We are looking for git-annex experts and novices alike - and everything in between. If you saw "git-annex" and thought "uuhhhh, interesting :thinking:" then come get on board!
- **Knowledge about HTTP requests/authentication**

But beyond this, if you have any additional idea or skill, just approach us! We look forward to hacking with you. :blush:


### Software setup: What do you need to install?

Here is a list of software that could be helpful to have installed for this project:
- [Git](https://git-scm.com/)
- [git-annex](https://git-annex.branchable.com/install/)
- [Python 3](https://www.python.org/downloads/)


### Code of conduct

As part of the Brainhack, this project adheres to the [OHBM's Code of Conduct](https://ohbm.github.io/hackathon2020/coc/). We ask all team members to respect and adhere to it, and to report code of conduct violations you encounter via the general channels detailed in the CoC. Feel free to contact Adina (adina.wagner@t-online.de, @adswa) as the project lead of this brainhack project if there is something CoC-related you want to discuss with her first.

## Get in touch!

If you want to become a part of this project, we're super happy to welcome you here. Get in touch via our [Mattermost channel](https://mattermost.brainhack.org/brainhack/channels/git-annex-osf), meet up with others in our [video chat](https://meet.jit.si/hbm-git-annex-osf), or create an issue to introduce yourself.

## Where to find TODOs?

Let's try to create an issue for any TODO there is, and for any task a project team member is working on. Hopefully, we can avoid misunderstandings or duplication of work in this way.

This means:
- if you see that something needs to be done, first create an issue about it!
- if you are working on something, comment on the issue that you are working on it. Reach out to others if you need help by tagging them or chatting them up in the Mattermost channel. Try to keep communication public, else it will be hard for others to join in and help.
- if you have solved an issue (e.g., with a Pull Request), close the issue to mark this TODO as resolved



## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="http://www.adina-wagner.com"><img src="https://avatars1.githubusercontent.com/u/29738718?v=4" width="100px;" alt=""/><br /><sub><b>Adina Wagner</b></sub></a><br /><a href="#projectManagement-adswa" title="Project Management">📆</a> <a href="#maintenance-adswa" title="Maintenance">🚧</a> <a href="https://github.com/adswa/git-annex-remote-osf/commits?author=adswa" title="Code">💻</a> <a href="https://github.com/adswa/git-annex-remote-osf/commits?author=adswa" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/DorienHuijser"><img src="https://avatars1.githubusercontent.com/u/58177697?v=4" width="100px;" alt=""/><br /><sub><b>Dorien Huijser</b></sub></a><br /><a href="https://github.com/adswa/git-annex-remote-osf/commits?author=DorienHuijser" title="Documentation">📖</a> <a href="#projectManagement-DorienHuijser" title="Project Management">📆</a> <a href="#ideas-DorienHuijser" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-DorienHuijser" title="User Testing">📓</a> <a href="#maintenance-DorienHuijser" title="Maintenance">🚧</a></td>
    <td align="center"><a href="https://github.com/TheDragon246"><img src="https://avatars2.githubusercontent.com/u/63247401?v=4" width="100px;" alt=""/><br /><sub><b>Ashish Sahoo</b></sub></a><br /><a href="https://github.com/adswa/git-annex-remote-osf/commits?author=TheDragon246" title="Documentation">📖</a> <a href="#maintenance-TheDragon246" title="Maintenance">🚧</a></td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
