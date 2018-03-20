# Project folder outline  

__Adapted from Noble WS (2009) A Quick Guide to Organizing Computational Biology Projects. PLoS Comput Biol 5(7): e1000424__  

A possible example for an effective project directory structure that promotes reproducible research. All the data and scripts to create the complete manuscript should be in this folder. Once your project is finished the complete directory should be set to read-only.  

Briefly, the structure contains 5 folders (Data, Doc, Results, Scripts and Tmp).  
All the data, including the original raw data (downloaded from HPC without subsequent manipulation), will be stored in the Data directory. Keep in mind that you should be able to recreate your analysis in a reasonable time with the scripts and data stored in your project folder. So it's sometimes better to save an intermediary data frame too much than too little.  
The Doc directory is the home of (preliminary draft of) your manuscript. It also contains all your notes, presentations, posters, papers,... related to the project.  
Plots, figures and anything that can be considered a result should be stored in your Results folder.   
The Scripts directory, on the other hand, houses all the used analysis scripts (dated) used for the project. I also create my local r env here.  
Temporary files, finally should be saved in the Tmp folder.

## Some additional recommendations:

- Use R projects with Packrat (version control for your R and Bioconductor packages) for each project.
- Never save your R workspace
- Use YYYY-MM-DD format for dates in filenames
- Start logical numbering with 01, 02, ... and not 1, 2, ...
- - & _ in filenames can be used to recover metadata
- Start filenames with lowercase
