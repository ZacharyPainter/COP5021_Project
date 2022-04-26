# README

# PRE-REQUISITE
    C++ build tools, for compiling C++ programs
    scan-build, for executing static analyzer, and viewing logs
        To install:
        $sudo apt install clang-tools

        Refer to: https://clang-analyzer.llvm.org/scan-build.html
        for further instructions on scan-build

# COMPILING
    To compile the test programs, enter their respective folder and execute $make

# RUNNING STATIC ANALYSIS
    To run the static analysis, enter the folder for either program and execute $scan-build make
    This will generate a log file, if there are any errors detected.

# VIEWING STATIC ANALYSIS LOGS FOR OPEN-SOURCE PROJECTS
    Static Analsysis logs were generated for the open source project VLC and Inkscape. This source code for these projects and be downloaded seperately and have their own prerequisites, however the logs for these projects are included here, in the /logs directory. 

    To view these logs in detail, navigate to the /logs directory and execute:
    $scan-view "folder name"

    This will open a web browser containing a detailed breakdown of the bugs detected in the corresponding software