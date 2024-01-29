# interactive NFT trait generator (under construction/ not working yet)

## This program allows you to create a (photo) collection by entering categories and their attributes.
By typing in up to twenty main traits, the user can generate ...After all attributes are added, each attribute ..
The result is a pdf in which the images are directly based on the output.  At the end the user would have to take multiple selfportraits based on the given requirements and feed it back to the program to finally put everything together.

With this python script, you can automatically generate occurrence probabilities by manually entering your preferred attributes, as is common in the NFT world. The functionality is explained in more detail using an example.

## Application
### To run the file on Windows:
#### Step 1
1. Clone the directory to the script (unpacked folder).
2. Open the command prompt (windows: cmd / mac: terminal/ linux: sudo?)
3. change directory to the copied path
  >cd 'your directory'

4. fire first script
  >py scriptname.py

5. Enter all the data and hit “Enter”

#### Step 2

1. After all attributes have been saved in a new .md document you can begin to visualize this data to your liking. (An example follows at the end of the readme)

2. Now load all images into the attached “imge_data” folder and make sure that the images are numbered so that the number appears before the file name (image-1.jpg)

3. repeat 1.-3. in **step 1**.

4. Run the second script to combine the text and images into a PDF.
>py combine_data.py

5. Admire your work in the “pdfs” folder.

## Here is an example of entered data:
(Link)
Description = NFT collection of photographically realized self-portraits in the rave milieu.
Title = Disco Portraits;
Author = Jasper V.;
Number of Trait types = 20;
Trait types: Background, Hair, Lipstick…
**This input represents the constant values, the trait types. Currently up to twenty of these can be entered**

Traits for “Background” (sorted from rare to common): golden, silver, blue, red, black, green…
**Here we only asked for the individual attributes for each zrait type. In this example, gold would be given the rarest probability of occurrence and green the most common probability of occurrence. However, the actual values are randomly generated, so the values are not too predictable.

This step is then repeated for each trait type until all traits have been defined for all trait types. This creates the NFT characteristic trading card logic with rare and common images**

## Libraries 
- FPDF
- numpy

## Found a bug?
If you encounter any bugs or other problems, please feel free to open an issue. Otherwise feel free to copy the repo, change the name and customize the script to your personal needs.

## Issues (work in progress)
- make the font choosable
- make more than 20 trait types possible
- add gui
