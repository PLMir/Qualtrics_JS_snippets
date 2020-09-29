# A few useful JS snippets for Qualtrics

How to use these snippets:
1. In the options wheel for a question, select "Add Javascript."
2. Include the code snippet below the line that reads "	/*Place your JavaScript here to run when the page loads*/"
3. Save and test with the Preview functionality. 

## Include a fixed question inside a Loop and Merge (loop_fixed)
Example use case: you want to add an attention check question midway through a loop and merge. 

1. At the top of the suvery flow, add an embedded data block and set a variable named "loop_number" to have the value 0. 
2. Add the Javascript code snippet "loop_fixed" to the first question of the block on which you are using Loop and Merge. 
3. Add a Display logic that will display your attention check question. Select "Embedded Data" on the first drop-down menu, loop_number as the embedded data variable and "is equal to" the loop after which you want your attention check question to be displayed. 


## Sampling without replacement (simple example)
Example use case: you have a 2 (condition A) x 2 (condition B)  design and 4 vignettes with one version of each vignette for each cell of the design. 
