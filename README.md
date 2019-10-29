# gitflow4code
## gitflow-avh Implementation for Visual Studio Code
This extension adds support for the feature branching strategy described here in [Vincent Driessen's branching model](http://nvie.com/posts/a-successful-git-branching-model/). The implementation used by this extension is similar to the functionality offered by [git-flow (AVH Edition)](https://github.com/petervanderdoes/gitflow-avh).

### What's included
* Initialize a repository with default or custom values for branch naming (i.e. 'develop', 'master', 'feature/', etc)
* Start/Finish Feature branches from "development", or from other branch bases
* Start/Finish Release branches from "development", or from other branch bases
* Start/Finish Hotfix branches from "production", or from other branch bases
* Get the status of a git repository

#### Dependencies
* git (if you have installed VS Code, this should also already exist on your machine)

# Getting Started
## Accessing gitflow4code commands
From the Command Pallette, type in GitFlow to filter the GitFlow commands

![GitFlow Command](images/FinishFeature.png)

## Initialize
Choose the Initialize Repository command from the list of available gitflow4code commands.

![Available GitFlow Commands](images/Initialize-Command.png)

Alternately, you can use the shortcut keys listed below
##### Shortcuts to Initialize Command
* ⌥⌘/ i on Mac
* Ctrl+Alt+/ i on Windows

### Initialize with default settings
Choose to `Initialize with default` (i.e. `master`, `develop`, `feature/`, `release/`, & `hotfix/`)

![Initialize with default](images/InitializeWithDefault.png)

### Initialize with custom configuration settings
Choose to `Initialize with custom values` and then specify the values requested

![Initialize master](images/MasterBranch.png)
![Initialize develop](images/DevelopBranch.png)
![Initialize feature](images/FeatureBranch.png)
![Initialize release](images/ReleaseBranch.png)
![Initialize hotfix](images/HotfixBranch.png)

These settings are stored and can be edited at any time by re-running the above commands or by editing in the Settings file.

![custom settings](images/InitializeSettings.png)


## Features
### Start Feature
Choose the `Start Feature` command from the list of available gitflow4code commands

![Features Command](images/StartFeature-Command.png)

Alternately, you can use the shortcut keys listed below
##### Shortcuts to Start Feature Command
* ⌥⌘/ f on Mac
* Ctrl+Alt+/ f on Windows

If creating a feature branch off of your development branch, choose `Start Feature from <develop>` (where `develop` is the name of whatever you chose to initialize your development branch) 

![Start Feature](images/StartFeatureDevelop.png)

 -- or --

If creating a feature branch off another base branch, choose `Start Feature from another base branch`

![Start Feature from another base branch](images/StartFeatureBase.png)


Then supply the name of your feature branch, and the tool will prefix it with whatever you chose to be the name of your feature branches

![Feature Name](images/FeatureName.png)

### Finish Feature
When finished with your feature, choose the `Features` command from the list of available gitflow4code commands and then choose to `Finish Feature` 

![Finish Feature](images/FinishFeature.png)

Alternately, you can use the shortcut keys listed below
##### Shortcuts to Finish Feature Command
* ⌥⌘/ ⌘f on Mac
* Ctrl+Alt+/ Ctrl+f on Windows

Or, use the Finish Feature button in the status bar

![Finish Feature](images/FinishFeature-Statusbar.png)

## Releases
### Start Release
Choose the `Releases` command from the list of available gitflow4code commands

![Releases Command](images/StartRelease-Command.png)

Alternately, you can use the shortcut keys listed below
##### Shortcuts to Start Release Command
* ⌥⌘/ r on Mac
* Ctrl+Alt+/ r on Windows

If creating a release branch off of your development branch, choose `Start Release from <develop>` (where `develop` is the name of whatever you chose to initialize your development branch) 

![Start Release](images/StartReleaseDevelop.png)

 -- or --

If creating a release branch off another base branch, choose `Start Release from another base branch`

![Start Release from another base branch](images/StartReleaseBase.png)

Then supply the name of your release branch, and the tool will prefix it with whatever you chose to be the name of your release branches

![Release Name](images/ReleaseName.png)

### Finish Release
When finished with your release, choose the `Releases` command from the list of available gitflow4code commands and then choose to `Finish Release` 

![Finish Release](images/FinishRelease.png)

Alternately, you can use the shortcut keys listed below
##### Shortcuts to Finish Release Command
* ⌥⌘/ ⌘r on Mac
* Ctrl+Alt+/ Ctrl+r on Windows

Or, use the Finish Release button in the status bar

![Finish Release](images/FinishRelease-Statusbar.png)

Then supply the name of the `Tag` for this release

![Tag Release](images/TagRelease.png)

## Hotfixes
### Start Hotfix
Choose the `Hotfixes` command from the list of available gitflow4code commands

![Hotfixes Command](images/StartHotfix-Command.png)

Alternately, you can use the shortcut keys listed below
##### Shortcuts to Start Hotfix Command
* ⌥⌘/ h on Mac
* Ctrl+Alt+/ h on Windows

If creating a hotfix branch off of your production branch, choose `Start Hotfix from <master>` (where `master` is the name of whatever you chose to initialize your production branch) 

![Start Hotfix](images/StartHotfixMaster.png)

 -- or --

If creating a hotfix branch off another base branch, choose `Start Hotfix from another base branch`

![Start Hotfix from another base branch](images/StartHotfixBase.png)

Then supply the name of your hotfix branch, and the tool will prefix it with whatever you chose to be the name of your hotfix branches

![Hotfix Name](images/HotfixName.png)

### Finish Hotfix
When finished with your hotfix, choose the `Hotfixes` command from the list of available gitflow4code commands and then choose to `Finish Hotfix` 

![Finish Hotfix](images/FinishHotfix.png)

Alternately, you can use the shortcut keys listed below
##### Shortcuts to Finish Hotfix Command
* ⌥⌘/ ⌘h on Mac
* Ctrl+Alt+/ Ctrl+h on Windows

Or, use the Finish Hotfix button in the status bar

![Finish Hotfix](images/FinishHotfix-Statusbar.png)

Then supply the name of the `Tag` for this hotfix

![Tag Hotfix](images/TagHotfix.png)


## Git Status
Choosing this from the gitflow4code commands list will display the current status of the local git repository (same as if running `git status` on the command line) and displays it in the `OUTPUT` pane

![Git Status](images/GetStatus-Command.png)

Alternately, you can use the shortcut keys listed below
##### Shortcuts to Start Hotfix Command
* ⌥⌘/ s on Mac
* Ctrl+Alt+/ s on Windows

![Git Status Result](images/GetStatus-Result.png)


# gitflow4code roadmap
See our [enhancements list](https://github.com/Shaggy13spe/gitflow4code/issues?q=is%3Aopen+is%3Aissue+label%3Aenhancement) for future plans


## Help Out?
This project is under constant development. Feedback and suggestions are very welcome and I encourage you to use the [Issues](https://github.com/Shaggy13spe/gitflow4code/issues) list on Github to provide that feedback.

### Contributing
Fork the repository and then run:
```sh
$ git clone -b master git@github.com:<username>/gitflow4code.git
cd gitflow4code
```

The `-b master` switch has to be added since the fork operation automatically clones the `develop` branch of the repository and cloning it results in a local repository with just a `develop` branch.

After that, initialize the local gitflow4code repository with `gitflow4code` itself (see Getting Started above).
Then create a feature branch, do your work and commit your changes publishing your feature branch.

When done, open a pull request to your feature branch.




