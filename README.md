![](Smithers_Logo.png)

# 1. Hamilton-Documentation

## Table of Contents
- [1. Hamilton-Documentation](#1-hamilton-documentation)
  - [Table of Contents](#table-of-contents)
  - [1.1. Setting up the Hamilton Access](#11-setting-up-the-hamilton-access)
  - [1.2. Before Running the Hamilton](#12-before-running-the-hamilton)
  - [1.3. Running a Method on the Hamilton](#13-running-a-method-on-the-hamilton)
- [2. Components of a Hamilton Method](#2-components-of-a-hamilton-method)

## 1.1. Setting up the Hamilton Access

- Have a bridge account with access to the Hamilton Method Manager, Hamilton Method Editor, and Hamilton Daily/Weekly Maintenance

- Have physical connection with the Hamilton machine

<p>&nbsp;</p>

## 1.2. Before Running the Hamilton
Every day run the Hamilton Maintenance program and go through this checklist
* - [ ] Make sure the machine is turned on. Blue light indicates machine is on and motors are engaged. Do **not** attempt to move the pipetting channels when the machine is on. If channels need to be moved, turn the machine off.
* - [ ] Check to see if daily or weekly maintenance must be done
* - [ ] Run the respective maintenance programs if needed. This is shown in bold red **REQUIRED** in the software


<p>&nbsp;</p>

## 1.3. Running a Method on the Hamilton

- Access the Hamilton Method Manager 
- Select method from 'Hamilton Standard Method' list
- Click on a method
- Select **Run Method**

<p>&nbsp;</p>

# 2. Components of a Hamilton Method

Every Hamilton method has several files that *must be* linked together

These files are the following

| File Name             | File Description                      | File Type |
|:----------------------|:-------------------------------------:|----------:|
| Hamilton Header File  | Compiled code generated to run machine| .hsl      |
| Hamilton System Deck  | Deck layout for the method            | .lay      |
| Hamilton Method       | Contains GUI-based Hamilton Method    | .med      |
| Hamilton RES File     | Helper file for the Hamilton Method   | .res      |
| Hamilton Method Data  | Helper file for the Hamilton Method   | .stp      |
| Hamilton SUB File     | Helper file for the Hamilton Method   | .sub      |

The most important methods are the System Deck, HSL Method, and Method files.
<p>
System Deck:    Contains layout of deck objects used for the respective Hamilton Method file and is linked with Hamilton Method file

Hamilton HSL Method:    Stands for 'Hamilton Standard Language' and is the underlying programming language for the machine. Contains all the necessary auxilliary libraries needed to run the Hamilton method and is also used to *generate* libraries. 

Hamilton Method:    Contains the actual **code** that the Hamilton processes to run the method.
