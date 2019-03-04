# The Basics

## Storing and building code

Source code is text files containing programming language statements. These files are stored in a Version Control System (VCS), which keeps an historical record of the line-by-line changes in each file stored in the VCS.

### Git!

(This is not an admonishment.) Git is a Distributed VCS (don't worry about the Distributed bit for now) - and GitHub is a service that provides it. [Use the GitHub learning resources](https://try.github.io/) to learn how to use Git. Some key terms to learn and understand are 'clone', 'commit', 'push', 'merge' and 'rebase'.

    Task: Add a link to an online tutorial that you have enjoyed, and add yourself to the contributors file.		

1. Fork this repository
2. Clone your copy of the repository
3. Add a tutorial link to [Useful-Tutorials.md](./Useful-Tutorials.md)
4. Add your name to the [Contributors.md](./Contributors.md) file.
5. Commit the changed files.
6. Push them to your repository.
7. Submit a pull request to the upstream repository (this one!)

### Build Automation

For languages that run on the Java Virtual Machine (JVM), (Java, Kotlin, Scala, and Groovy to name a few), there are several build tools to choose from. Maven is by far the most popular, but Gradle, SBT and Bazel are also modern alternatives. Ant and Ivy are from an older generation of build tool, but can still be found in use.

#### Maven

[Apache Maven](https://maven.apache.org/) is an Open Source build tool, with an XML-based configuration system.

 - [Getting started](https://maven.apache.org/guides/getting-started/)
 - [Maven in 5 minutes](https://maven.apache.org/guides/getting-started/maven-in-five-minutes.html)

#### Gradle

[Gradle](https://gradle.org/) is an Open Source build tool, with a Groovy or Kotlin based configuration system.

 - [Gradle Guides](https://gradle.org/guides/)

#### Command Wrappers

Gradle and Maven both support 'command wrappers', a minimal library and script which are stored in a VCS along with the source code.

Command wrappers allow source code authors to easily specify the version of a build tool in use. The script will install the full build tool if it's not already installed, it provides contributors with an easy way to get up and running with a given code base.

 - [Maven Wrapper](https://github.com/takari/maven-wrapper)
 - [Gradle Wrapper](https://docs.gradle.org/current/userguide/gradle_wrapper.html)

### CI

Continuous Integration (CI) is the practice of merging new source code into the main code base at least once per day.

When source code is committed to a central repository, it can be automatically compiled, tested and packaged. Automation can be used to check code quality, formatting styles and correctness, then to send feedback to source code authors about their work.
