## 1. Download and install [devkitPro](https://github.com/devkitPro/installer/releases).

**a.** Open the devkitProUpdater.exe file and let it install what it wants to.

![image](https://user-images.githubusercontent.com/17243618/122804473-f5290b80-d295-11eb-9b1e-f8ce46300ff0.png)

***

**Note**: If you just started following this tutorial, ignore this note for now. If you see compile warnings when building a fresh CFRU or Ability Pop-Ups crash your game after the build process is finished, download from [this link](https://www.mediafire.com/file/br2xpo14rd2a76c/devkitPro.zip/file) instead. Replace the devkitPro folder created when you installed devkitPro before (likely ``C:/devkitPro``) with the contents of the downloaded archive.

![image](https://user-images.githubusercontent.com/17243618/122796738-bc386900-d28c-11eb-9508-c0e4f5916595.png)

## 2. Add devkitARM's bin folder to your path.

**a**. Open ``This PC``. Right-click on the background and choose ``Properties``.

![image](https://user-images.githubusercontent.com/17243618/122797091-1a654c00-d28d-11eb-88b2-11ebf4583bff.png)

***

**b**. On the sidebar, click ``Advanced System Settings.``

![image](https://user-images.githubusercontent.com/17243618/122797333-60221480-d28d-11eb-96a5-1b57ffa140ef.png)

***

**c.** In the pop-up window, click ``Environment Variables``.

![image](https://user-images.githubusercontent.com/17243618/122798162-446b3e00-d28e-11eb-8c53-dadbb7c6214f.png)

***

**d.** In the next pop-up window, find ``Path`` under ``System variables`` at the bottom and click ``Edit``.

![image](https://user-images.githubusercontent.com/17243618/122805114-acbe1d80-d296-11eb-86cf-66bf999400eb.png)

***

**e.** In this final pop-up window, click ``New`` and add devkitARM's ``bin`` folder. Most likely this will be at ``C:\devkitPro\devkitARM\bin``.

![image](https://user-images.githubusercontent.com/17243618/122799125-5c8f8d00-d28f-11eb-9d94-0bd642d022db.png)

***

**f.** Hit okay on everything to save and close it all.

## 3. Download and install [Python 3.7.6](https://www.python.org/downloads/release/python-376/).

**Note 1**: Make sure you allow Python to be added to your path as part of the installation. Otherwise, you will have to repeat step 2 for Python as well.

**Note 2**: **DO NOT DOWNLOAD PYTHON 3.8 OR HIGHER!**

## 4. Restart your computer.

This should be self-explanatory.

## 5. Download the CFRU.

**Option a.** On the [main page](https://github.com/Skeli789/Complete-Fire-Red-Upgrade), click ``Code`` and then or click ``Download Zip``.

![image](https://user-images.githubusercontent.com/17243618/122800746-50a4ca80-d291-11eb-8ccd-0f705d5203dd.png)

***

**Option b.** Download and install [git](https://git-scm.com/download/win), then open a command line and clone the repository with ``git clone https://github.com/Skeli789/Complete-Fire-Red-Upgrade.git``. This is the preferred method as you can easily retrieve updates from GitHub.

![image](https://user-images.githubusercontent.com/17243618/122801128-bee98d00-d291-11eb-98cd-285a568469b9.png)

## 6. Put your base ROM in the root.

**a**. Download a Pokemon FireRed 1.0 ROM. For legal reasons, no link will be provided.

**b**. Rename it to ``BPRE0.gba`` and place it in the root of the repository.

![image](https://user-images.githubusercontent.com/17243618/122801440-1be54300-d292-11eb-99e2-0f3bfbca3120.png)

## 7. Choose your insert offset.

**a**. If you don't know what this means, skip to the [next step](#8-run-the-make-script-from-the-root).

**b**. By default, the CFRU is compiled to the offset ``0x900000``. If you would like to change this, open ``scripts/make.py`` and change the line ``OFFSET_TO_PUT = 0x900000``.

## 8. Run the make script from the root.

**a**. Hold shift and right-click the background of the folder. In the context window pop-up, click ``Open command window here`` or ``Open PowerShell window here``.

![image](https://user-images.githubusercontent.com/17243618/122802750-bb570580-d293-11eb-9129-babdcaa08db7.png)

***

**b.** In the terminal that just opened, type ``python scripts/make.py``.

![image](https://user-images.githubusercontent.com/17243618/122803343-7a132580-d294-11eb-8d04-23f47874aca8.png)

***

**c.** Hit enter to run the script. When the build process is done, you should see something like this on the terminal:

![image](https://user-images.githubusercontent.com/17243618/122803778-13dad280-d295-11eb-8a8b-b3ad589bfbaa.png)

In addition, these files will also now appear in the root:

![image](https://user-images.githubusercontent.com/17243618/122803929-41278080-d295-11eb-9d10-f6e5e93d8ae0.png)

***

**Note 1**: If you get an error with a mention of a file called ``libwinpthread-1.dll`` (or something similar), search Google for a 64-bit version of this file and add it to the root.

**Note 2**: If you receive several compile warnings during the build process, see the note in the [first step](#1-download-and-install-devkitpro). 

## 9. Read the [documentation](https://github.com/Skeli789/Complete-Fire-Red-Upgrade/blob/master/CFRU%20Documentation.pdf) thoroughly.

Once you've done that, you're good to go! Enjoy using the Complete FireRed Upgrade!

## Other Links
If after following this tutorial you still are unable to use the CFRU, try watching [this video](https://www.youtube.com/watch?v=542jj04YZPE) instead.