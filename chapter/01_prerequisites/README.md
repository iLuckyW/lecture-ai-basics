# Prerequisites

Before setting up your environment, you need to clone the course repository to your local machine. Follow these steps:

1. **Check if Git is installed:**

    Open your terminal or command prompt and run:
    ```bash
    git --version
    ```
    If Git is not installed, download it from [https://git-scm.com/downloads](https://git-scm.com/downloads) and install it.

    **Optional**: If you prefer a graphical interface, install a [Git GUI](https://git-scm.com/downloads/guis) such as GitHub Desktop or use the built-in Git tools in Visual Studio Code.

2. **Choose a folder where you want to store the project**

     Cretae or navigate to that folder in your terminal, for example:
     ```bash
     mkdir -p ~/documents/uni/ai-course
     cd ~/documents/uni/ai-course
     ```


3. **Clone the repository using HTTPS or SSH**

    * **Using HTTPS (recommended if you don’t have SSH keys set up):**
        ```bash
        git clone https://github.com/Paul-B98/lecture-ai-basics.git
        ```
    *  **Using SSH (if you have SSH keys configured with GitHub):**
        ```bash
        git clone git@github.com:Paul-B98/lecture-ai-basics.git
        ```


4. **Navigate into the cloned repository folder and check the contents**
    ```bash
    cd lecture-ai-basics
    ls
    ```
    You should see files like README.md, environment files, and notebook folders.

## Setting Up Your Python Environment and Packages
After cloning the repository, set up your Python environment. You have two options:

### Option 1: Using Devcontainer (Recommended for VS Code Users)

1. **Ensure you have the following installed:**
    * [Docker](https://www.docker.com/)
    * [Visual Studio Code](https://code.visualstudio.com/)
    * **Optional (for Windows)** [WSL](https://learn.microsoft.com/de-de/windows/wsl/install)
    * **Optional (for Windows)** [Remote Development Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)

2. **Open the cloned repository folder in VS Code**

    You can opne VS Code by running `code .` in your terminal or by selecting **File > Open Folder...** in the VS Code menu.

3. **Reopen the project in a dev container:**
    - Option 1: Press `F1` to open the command palette, type `Remote-Containers: Reopen in Container`, and select it.
    - Option 2: When prompted, click **Reopen in Container**.

    VS Code will build the container based on the provided devcontainer.json and install all required dependencies automatically. Once setup is complete, your environment is ready, and you can run all notebooks directly within the container.

### Option 2: Using Anaconda (Cross-Platform Alternative)

1. **Ensure [Anaconda](https://www.anaconda.com/download) is installed.**

2. **Create a new conda environment**

    Open your terminal and run:
    ```bash
    conda create --name ai-course python=3.12
    ```

3. **Activate your environment**

    After creating the environment, activate it with:
    ```bash
    conda activate ai-course
    ```

4. **Install required packages**

    Navigate to the cloned repository folder and install the required packages using pip:
    ```bash
    pip install .
    ```

5. **Start Jupyter Lab**

    Run the following command to start Jupyter Lab:
    ```bash
    cd chapter
    jupyter lab
    ```

    This will open Jupyter Lab in your default web browser, allowing you to access and run the notebooks.

## Completing the Python Basics Subchapter

After setting up your environment, begin with the [Python Basics](./basics.ipynb) subchapter to ensure you have the necessary programming foundation for this module.
