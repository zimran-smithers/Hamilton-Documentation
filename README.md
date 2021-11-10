
# Hamilton-Documentation

Overview on how to use the Hamilton

### Setting up the Hamilton Access

- Have a bridge account with access to the Hamilton Method Manager,Hamilton Method Editor, and Hamilton Daily/Weekly Maintenance

- Have physical connection with the Hamilton machine

<p>&nbsp;</p>

# Before Running the Hamilton
Every day run the Hamilton Maintenance program and go through this checklist
- [ ] Check to see if daily or weekly maintenance must be done
- [ ] Run the respective maintenance programs if needed. This is shown in bold red **REQUIRED** in the software


<p>&nbsp;</p>

# Running a Method on the Hamilton

- Access the Hamilton Method Manager 
- Select method from 'Hamilton Standard Method' list
- Click on a method
- Select **Run Method**

<p>&nbsp;</p>

# Components of a Hamilton Method

Every Hamilton method has several files that *must be* linked together

These files are the following

| File Name             | File Description                      | File Type |
|:----------------------|:-------------------------------------:|----------:|
| Hamilton HSL Method   | Included libraries used in a method   | .hsl      |
| Hamilton System Deck  | Deck layout for the method            | .lay      |
| Hamilton Method       | Contains GUI-based Hamilton Method    | .med      |
| Hamilton RES File     | Helper file for the Hamilton Method   | .res      |
| Hamilton Method Data  | Helper file for the Hamilton Method   | .stp      |
| Hamilton SUB File     | Helper file for the Hamilton Method   | .sub      |

The most important methods are the System Deck, HSL Method, and Method files.
<p>
System Deck:    Contains layout of deck objects used for the respective Hamilton Method file and is linked with Hamilton Method file

Hamilton HSL Method:    Contains all the necessary auxilliary libraries needed to run the Hamilton method.

Hamilton Method:    Contains the actual **code** that the Hamilton processes to run the method.
