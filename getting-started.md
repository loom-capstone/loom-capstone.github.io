# Getting Started

This guide is intended for onboarding new Loom developers.

## Glossary

<dl>
    <dt>Arduino sketch</dt>
    <dd>An Arduino program file (<code>.ino</code>) that you write and upload to a microcontroller.</dd>

    <dt>Board package</dt>
    <dd>Describes how an Arduino sketch should be compiled and uploaded to a microcontroller. It specifies the target hardware, compilation settings, upload interface, and can include <a href="https://htmx.org/essays/vendoring/">vendored</a> libraries. Board packages are installed through the Arduino IDE board manager.</dd>

    <dt>Library</dt>
    <dd>A collection of C++ source files (<code>.cpp</code> and <code>.h</code>) that expose a public API to be used in an Arduino sketch.</dd>
</dl>

## Development Environment

Users of Loom (i.e. the teams within OPEnS Lab) install the latest version of the Loom by using the Arduino IDE board manager. However, as a Loom developer, you will want to work on features and fixes using local, version-controlled source files.

Now let's begin setting up a local development environment on your computer.

### Requirements

You must have the following software installed on your computer:

* [Arduino IDE](https://docs.arduino.cc/software/ide/)
* [Git](https://git-scm.com)

### Creating Your Development Environment

1. Navigate to the [Arduino Sketchbook folder](https://support.arduino.cc/hc/en-us/articles/4412950938514-Open-the-Sketchbook-folder). This is typically `~/Arduino` or `~/Documents/Arduino`.

    ```
    cd ~/Documents/Arduino
    ```

2. Create the `libraries` folder if it does not already exist and navigate into that folder.

    ```
    mkdir -p libraries && cd libraries
    ```

3. Clone the Loom library into the `libraries` folder. Name it something like `Loom-dev` so you can easily differentiate it from the library installed with the Loom board package.

    ```
    git clone https://github.com/OPEnSLab-OSU/Loom-V4.git Loom-dev
    ```

    **Note:** Placing a library in your sketchbook's `libraries` folder overrides other installed versions of that library.

That’s it! You now have a local development environment for working on Loom.

## Testing Changes

While you are working on bug fixes and features, it is a good idea to regularly test your code on hardware.

*Under construction...*
