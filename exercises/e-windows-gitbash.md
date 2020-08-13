## Add `make` to Git Bash
# -------------------------

Follow [these instructions](https://gist.github.com/evanwill/0207876c3243bbb6863e65ec5dc3f058); specifically the **make** section. You will download a `zip` file, extract, and copy those files to `C:\Program Files\Git\mingw64\` *without* overwriting any files.

This will allow you to run `> make` from Git Bash within the `data-science-curriculum`, which will process the exercises. However, the final step of `make` will fail unless you also install Python.

## Install Python (Highly recommended)
# -------------------------

Installing Python is optional but *highly recommended*; this will create a set of exercises in `exercises_sequenced` that have a prefix `dXY-` for the *day* associated with that exercise (e.g. `d03-` means day 3 of the class).

- Download and install [Python](https://www.python.org/downloads/) for Windows.
- Once installed, determine the `path` of your Python executable.

1. Press the Windows key, type `python`, and click the "open file location" button.

![python location](./images/python-location.png)

2. It's likely that this is *not actually Python*! Instead, it's a shortcut. Click on *Properties* so we can see where this shortcut points.

![python properties](./images/python-properties.png)

3. This will bring up a menu with a `Target` field that ends with `python.exe`. Everything that comes before `python.exe` is the **path** of that file. Copy that text, and be ready to paste it into another file.

![python target](./images/python-target.png)

- Download the example `.bashrc` file, and save it to your *home directory*. This is usually `C:\Users\username`; for example, my home directory is `C:\Users\zdelrosario`.

- Copy the **path** for Python into that example `.bashrc` file (you can use notepad to edit it), following the instructions to edit the `export PATH="$PATH:/stuff"` line.

- In Git Bash, change directories to the `data-science-curriculum` and try to run `make`. If Python is installed correctly, then you should see a bunch of stuff fly by in Git Bash, and the folder `exercises_sequenced` should fill with exercises.

If you have **any** issues with these steps, please reach out to one of the teaching staff!
