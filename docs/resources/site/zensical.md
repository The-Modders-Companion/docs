---
icon: simple/zensical
---
# Zensical

My website is powered by [Zensical](https://zensical.org/), a static site generator. Zensical was created by the team behind [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) and is geared toward documentation sites. Currently, Zensical is in alpha.

This page explains how to set up Zensical and this website on a new machine. It is mostly for my personal benefit ~~because my brain consists of swiss cheese~~.

## How to set up the site

The [Zensical documentation](https://zensical.org/docs/get-started/) also details the setup process. However, you can find all relevant information for a setup on Windows here.

### Installing Python

You can skip this step if you have already installed Python on your PC.

- Download the latest version of [Python for Windows](https://www.python.org/downloads/) from the official website.
- Run the downloaded file to install Python.

The terminal will open (see the screenshot below).

- Enable long path support. 
- Do not add Python to PATH.
- Confirm to install the latest version of Python.
- Restart your PC.

![Python Setup](python-setup.png)

### Cloning the repository

- Install [Git](https://git-scm.com/install/windows) if you haven't done so already.
- Open the Command Prompt and run the following commands one by one:

```  { .yaml .annotate }
cd /d C:\ #(1)!
mkdir Drive:\My\Project\Folder
cd /d C:\Zensical
git clone https://github.com/The-Modders-Companion/docs.git .
```

1. Use this command to switch to the top level of the drive on which you would like to set up the project folder. The argument `/d` is necessary to switch between drives. `C:\` can be any drive letter.

### Installing Zensical

Finally, install Zensical into the new project folder:

- Run the following commands one by one in the Command Prompt while in the project folder directory:

```
python -m venv .venv
.venv\Scripts\activate
pip install zensical 
```

### Running Zensical

Every time you want to run Zensical locally, you need to open the Command Prompt, navigate to the project folder, and run the following commands:

```
.venv\Scripts\activate
zensical serve
```

## How to update Zensical

Instructions on how to update Zensical can be found on the [official website](https://zensical.org/docs/upgrade/) and the changelog is [here](https://github.com/zensical/zensical/releases).

To check the currently installed version, run:

```
pip show zensical
```

To update Zensical, run:

```
pip install --upgrade --force-reinstall zensical
```

## How to create a new branch

When working on a different part of the site, create a new branch.

```
cd /d Drive:\Project Folder
.venv\Scripts\activate
git switch main
git pull
git switch -c [branch-name]
```

Use the following commands for branches:

- `git branch` - Display currently active branch
- `git switch [branch]` - Switch to a different branch (**commit first**)

### Merge branch into main

```
git switch main
git pull
git merge [branch-name]
git push
```

### Delete branch

```
git switch main
git pull
git branch -d [branch-name]
git push origin --delete [branch-name]
```

## Zensical Commands

* [`zensical new`][new] - Create a new project
* [`zensical serve`][serve] - Start local web server
* [`zensical build`][build] - Build your site

  [new]: https://zensical.org/docs/usage/new/
  [serve]: https://zensical.org/docs/usage/preview/
  [build]: https://zensical.org/docs/usage/build/

## .gitignore Configuration

The repositor already has a `.gitignore` but here are the instructions for posterity:

- In the project folder, create a `.gitignore` file.
- Open your `.gitignore` in Notepad or similar and paste the following:

```yaml
.venv/
/site/ #(1)!
```

1. Starting with a backslash is necessary to specify the top-level `site` folder and avoid excluding any other folders with the same name.

Save and close the file.

## Plugins

### Awesome Nav

See [Awesome Nav](https://zensical.org/docs/compatibility/mkdocs/plugins/#awesome-nav) in the official Zensical documentation or refer to the [original plugin's documentation](https://lukasgeiter.github.io/mkdocs-awesome-nav/).

- Enable the plugin by adding `[project.plugins.awesome-nav]` to the `zensical.toml`.
- Create a `.nav.yml` file inside `\docs\`.

This file determines the order of tabs in the top navigation.

```yaml
site:
    resources
    blog
```
Then create folders and sub-folders for each section and page:

```
docs/
├─ .nav.yml
└─ resources/
   └─ site/
        └─zensical.md
└─ blog/
   └─ index.md
```