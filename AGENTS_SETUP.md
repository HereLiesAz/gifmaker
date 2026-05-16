# Project Setup Instructions

This document provides a brief overview of how to initialize the development environment for this repository. For comprehensive rules, guidelines, and project architecture details, please consult `AGENTS.md` and the exhaustive documentation located in the `/docs/` directory.

## Environment Setup

To begin development, you must configure your local environment to support Android builds.

1.  **Run the Setup Script**: We provide an automated bash script that handles the installation of necessary dependencies, including Java (JDK 17) and the Android SDK.

    ```bash
    ./setup_env.sh
    ```

2.  **Verify Setup**: The script will append necessary environment variables (like `ANDROID_HOME`) to your `~/.bashrc`. If you do not use bash, or if the script fails to update your profile, ensure the following variables are set manually:
    *   `ANDROID_HOME` pointing to your Android SDK installation.
    *   `ANDROID_SDK_ROOT` pointing to the same location.
    *   Update your `PATH` to include the `cmdline-tools/latest/bin` and `platform-tools` directories within the SDK.

**Note for AI Agents**: If you encounter environment issues, run `./setup_env.sh` and carefully read its output before attempting manual interventions.