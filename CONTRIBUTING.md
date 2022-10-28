# Contribute to CodeEdit

## Initial Steps & Getting Acquainted

### Summary and Quick Start

1. To get started with CodeEdit, please read the [Getting Started](https://github.com/CodeEditApp/CodeEdit/wiki/Getting-Started) guide in our wiki.

1. Installation: Fork & Clone the CodeEdit Repository.

1. Install SwiftLift before building the project in Xcode. Please read the SwiftLint section in our [Code Style](https://github.com/CodeEditApp/CodeEdit/wiki/Code-Style) guide for details.

1. Open the Project in Xcode. Open the `CodeEdit.xcworkspace` file, NOT `CodeEdit.xcodeproj`

1. Review the [Troubleshooting](https://github.com/CodeEditApp/CodeEdit/wiki/Troubleshooting) guide that provides common resolutions for errors encountered when trying to build the project.

1. Explore items to work on in the [Issues tab](https://github.com/CodeEditApp/CodeEdit/issues)

1. Submit a detailed Pull Request with all template fields populated.

1. Request a review from one of our admins/maintainers: @austincondiff, @lukepistrol, @MarcoCarnevali, @jasonplatts, @pkasila, @cstef, @linusS1, @RayZhao1998, @wdg

### Installation

While additional information is dispersed across the [Getting Started](https://github.com/CodeEditApp/CodeEdit/wiki/Getting-Started), [Code Style](https://github.com/CodeEditApp/CodeEdit/wiki/Code-Style), and [Troubleshooting](https://github.com/CodeEditApp/CodeEdit/wiki/Troubleshooting) guides, please follow the concise steps below to get up & running with CodeEdit in Xcode.

#### Fork & Clone CodeEdit

To contribute/make changes, you will need to fork the CodeEdit repository. A fork is a copy of a repository. Forking a repository allows you to freely experiment with changes without affecting the original project.

To fork the CodeEdit repo, click the **"Fork"** button in the banner to the top right. After forking, clone the forked repository to your Mac.

For detailed instructions see official guide [here](https://docs.github.com/en/get-started/quickstart/fork-a-repo).

#### Install SwiftLint

To enforce our style we settled on, we use a tool called [SwiftLint](https://github.com/realm/SwiftLint) It gets executed at build time and injects error messages right into Xcode.

You can install it using [Homebrew](http://brew.sh/) in Terminal:
```bash
brew install swiftlint
```

#### Open the Project in Xcode

> **Important:** Make sure you have at least `macOS 12 Monterey` installed since our deployment target is `macOS 12`. Otherwise the project will not build and run properly!

Now that you've forked and cloned the CodeEdit repository, you have everything you need to get started (assuming you already have everything setup for Xcode. If not, follow install instructions from the official site [here](https://developer.apple.com/xcode/)).

Navigate to the directory where you cloned the repository to in Finder. Inside that directory you will find a couple of files and sub-directories.

You want to open the `CodeEdit.xcworkspace` file in Xcode.

![CodeEdit.xcworkspace](https://user-images.githubusercontent.com/9460130/158924759-42a61d23-4961-4bfb-8d44-930ec2427f0f.png)

> Note: Do not open the `CodeEdit.xcodeproj` file since it will not include our internal modules which are required to build & run CodeEdit.

### Communication

We use Discord extensively. Please join the [Discord Server](https://discord.gg/vChUXVf9Em) to ask questions, collaborate with others, and access additional resources related to CodeEdit.

## Explore Issues

Find issues from the [Issues tab](https://github.com/CodeEditApp/CodeEdit/issues) or from the To Do column in our [project](https://github.com/orgs/CodeEditApp/projects/3/views/2). If you find an issue you want to work on, please indicate it in the issue and/or attach a draft PR once available. An admin or maintainer will then assign the Issue and/or PR to you.

> ⚠️ Please do not submit `localization` related pull requests at this time.
> Once we are ready to support more languages we will let you know with a guide on how to contribute here and on our [Discord Server](https://discord.gg/vChUXVf9Em).

## Submitting a Pull Request

Once you are happy with your changes, you will submit a `Pull Request`.

The pull request opens with a template loaded. Fill out all fields that are relevant.

The `PR` should include following information:
* A descriptive **title** on what changed.
* A detailed **description** of changes.
* If you made changes to the UI please add a **screenshot** or **video** as well.
* If there is a related issue please add a **reference to the issue**. If not, create one beforehand and link it.
* If your PR is still in progress mark it as **Draft**.

### Checks, Tests & Documentation

Request a review from one of our admins @austincondiff, @lukepistrol, @MarcoCarnevali, @jasonplatts, @pkasila or maintainers @cstef, @linusS1, @RayZhao1998, @wdg.

Note: If it is your first PR, an admin will need to request a review for you.

> Please resolve all `Violation` errors in Xcode (except: _TODO:_ warnings). Otherwise the swiftlint check on GitHub will fail.

Once you submit the `PR` GitHub will run a couple of actions which run tests and `SwiftLint` (this can take a couple of minutes). Should a test fail, it cannot be merged until tests succeed.

Make sure to resolve all merge-conflicts otherwise the `PR` cannot be merged.

> **Important**: make sure your code is well documented so others can interact with your code easily!
