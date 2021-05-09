## Contributing figure code

1. [Clone](https://happygitwithr.com/rstudio-git-github.html) or pull the most recent version of this repository from GitHub.

2. Create the plot in a new Rmd using `template.Rmd`.
    - Open `template.Rmd` and save in the appropriate folder (e.g. "general", "spatial") with an informative name (e.g. `facetted_boxplots.Rmd`).
    - If necessary, save your dataset(s) in the same folder with the same title as the Rmd, appended by "data" (e.g. `facetted_boxplots_data.csv`).
    - Update the YAML header (title, author name and email).
    - Add a description of the figure, with any notes that may be useful (e.g. links to associated resources, suggested statistics, citation for the published version).
    - Copy your figure code into the Rmd, make sure everything works, and annotate the code.

3. Knit your new Rmd.
    - This will generate an HTML document as well as a figure in the `figures` folder.

4. Reference your figure in the README.
    - Open `README.Rmd`.
    - Copy this code chunk into the appropriate section and update to match your figure's title and your Rmd's file path.

```{r}     
insert("Cool Boxplots", "general/facetted_boxplots.Rmd")    
```
    
5. Knit `README.Rmd`.
    - This will update the README displayed on GitHub (`README.md`).
    
6. Save your Rmd and README.Rmd. Commit everything and push to the GitHub repository.

*Need to troubleshoot, install, or just figure out how to to use Git with R? Check out [Happy Git and GitHub for the useR.](https://happygitwithr.com)*
