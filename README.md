# Lab exercise 1 objectives
1. Navigate and explore Tuffix, a Linux environment.
2. Write C++ code on the Atom editor.
3. Navigate the Linux file system using a command line interface (CLI).
4. Compile C++ code.
5. Run compiled code (executable files).
6. Use git to add and commit code to the local staging area as well as push code to a Github repository.

# Instructional videos
Here are some instructional videos that you can view to know more about Tuffix and the command line.
1. Running Tuffix using Virtual Box (https://youtu.be/otB9FPC86a8?t=1m54s)
2. Intro to Tuffix (https://youtu.be/c0ZrWmarSwI)
3. Intro to the Linux command line (https://youtu.be/bQm8TUTDK7E)
4. Intro to Atom and g++ compilation (https://youtu.be/TYlg3Ka8Mos)

# Instructions
Follow the steps listed below to complete this lab exercise.
1.  Make sure that the shared clipboard of VirtualBox is set to *Bidirectional* to allow you to easily copy and paste text between your host operating system and your virtual machine.
 ![Setting shared clipboard to bidirectional](https://raw.githubusercontent.com/CSUF-CPSC121-2018F01-04/labex1/master/screenshots/Shared%20clipboard.png?token=AAU0CfpIIyiAVj5nK0w8ytC8GJmH83Z2ks5bjrFTwA%3D%3D)
1. Make a copy of this Github repository on your computer using the `git` command. Add the `clone` command and a URL to specify where it can get a copy of the repository. You can find the URL by clicking on the green *Clone or download* button at the top right part of this page. Copy the URL and replace the dummy text shown below. When you hit <kbd>Enter</kbd> it will ask you to provide your Github username and password. Provide the information to start the cloning process. Once done, you will have a copy of the repository on your computer.
 
    ```
    git clone <place URL here>
    ```
1. Navigate into your labex1 folder using the command line. Take note that this will vary per user because the folder name is based on your Github username. The example below assumes the user's username is Tuffy. Replace it with your own folder name. Take note that you can type the first few letters of the folder name and press <kbd>Tab</kbd> so that it auto completes the folder name for you.

    ```
    cd labex1-tuffy
    ```
1. Provide your Github username and password when asked.
1. You should now have a copy of the files on your machine. Use the Atom editor to create a file called hello.cpp that will print *Hello world* on the screen.
1. Compile the file using the command below

    ```
    g++ -std=c++14 hello.cpp -o hello
    ```
1. Run the program using the command below

    ```
    ./hello
    ```
1. If everything runs correctly, then let's copy your code into the repository. The first step is to add hello.cpp to what is called the staging area using git's add command. The parameter after add is the name of the file you want to add. Optionally, you can type . (period) if you want to add all modified files.

    ```
    git add hello.cpp
    ```
1. Once everything is in the staging area, we use the commit command to tell git that we have added everything we need into the staging area.

    ```
    git commit
    ```
1. In case it asks you  to configure global variables for an email and name, just copy the commands it provides then replace the dummy text with your email and Github username.

    ```
    git config --global user.email "tuffy@csu.fullerton.edu"
    git config --global user.name "Tuffy Titan"
    ```
1. Git will ask you to describe what you have added to the staging area. By default, you will use a command-line based editor called *nano*. Go ahead and provide a description then press <kbd>Ctrl</kbd> + <kbd>x</kbd> to exit. Finally press <kbd>Y</kbd> to confirm that you want to make changes.
1. Finally, lets push all changes to the Github repository using git push.

    ```
    git push
    ```
1. Congratulations! You have now created a C++ project on Github!
