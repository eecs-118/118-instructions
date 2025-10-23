# EECS 118 — Environment Setup (Windows 10 / 11)

## Install Python 3.12.1
1. Download **Python 3.12.1 (64-bit)** from:
   [https://www.python.org/downloads/release/python-3121/](https://www.python.org/downloads/release/python-3121/)

2. Run the installer → choose **Customize installation** →
   check **Add Python to PATH** → keep all defaults → finish installation.

## Install VSCode with Python Extensions

3. Download and install **Visual Studio Code** from:
   [https://code.visualstudio.com/](https://code.visualstudio.com/)

4. In VS Code, install the **Python** extension (it will automatically install **Pylance** and **Jupyter**).

## Create a new Workspace

5. Create an empty folder on your computer for the project
   (for example `C:\UCI\EECS118\Lab1`).

6. In VS Code, choose **File > Open Folder...** → select your project folder.

7. Choose **File > Save Workspace As...** → keep the default name and location.

8. Verify that you are in a workspace by checking that the VS Code window title ends with `.code-workspace`.

## Setup Python Virtual Environment

9. Open the Command Palette (`Ctrl+Shift+P` or `F1`) → search for
   **Python: Create Environment** → select **New virtual environment**,
   and choose **Python 3.12.1** as the base interpreter.

10. Choose **Venv**, keep the default folder name `.venv`,
    skip package installation, and wait for setup to finish.

11. Set the default terminal to **Command Prompt** (Ctrl+, → search for `terminal.integrated.defaultProfile.windows` → select **Command Prompt**)
    and close any open terminals.

12. Open a new terminal in VS Code by pressing **Ctrl+J**.

13. Verify that the prompt begins with `(.venv)`.

14. Run

    ```
    where python
    ```

    The first path should point to your project’s `.venv\Scripts\python.exe`.

15. Run

    ```
    python --version
    ```

    It should return **Python 3.12.1**.

16. Run
    ```
    pip install pygame numpy matplotlib gymnasium networkx pillow tqdm scipy pandas seaborn opencv-python
    ```
    to install python packages that we will need.

## Download and Run Source Code

17. Download the source code from **Canvas > Files**
    and unzip it **into your project folder** (not a subfolder).

18. In VS Code, open `main.py` and run it using

    ```
    python main.py
    ```

    or click **Run ▶** at the top of the editor.
