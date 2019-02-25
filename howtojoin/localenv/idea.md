# Install and setup IntelliJ IDEA

## Install

Download and execute installer to your pc.

IntelliJ IDEA:  
https://www.jetbrains.com/idea/

Usually install Community Edition.
If you have Ultimate license, you can install it.

## Install Plugins

Install 'Lombok Plugin', following process.

- Start IntellJ IDEA
- Select Configure -> Plugins.
- Push 'Browse repositories'.
- Search 'Lombok Plugin', and select it.
- Push 'Install'.

## Setup Project

Start terminal, and clone Repository.

```sh
git clone git@github.com:<organization>/<repository>.git
```

Import project, following process.
- Start IntellJ IDEA
- Push 'Import Project'
- Select repository working directory.
- Select 'Import project from external model' -> 'Gradle', and Next.
- Check 'Use auto-import', and Finish.
- Read attention 'File Already Exists', and 'Yes'
- Wait for initialize and build project.

If you have problem with building.
- Open project directory with IntellJ IDEA
- Select 'File' -> 'Project Structure'
- Select 'Project' in 'Project Settings'
- Make sure Project SDK is set to java 1.8.

Back to terminal, and checkout codeStyle Directory.  
(you can use project standard code style in IntelliJ IDEA.)

```sh
git checkout .idea/codeStyles
```
