## Contributing figure code

1. [Clone](https://happygitwithr.com/rstudio-git-github.html) or pull the most recent version of this repository from GitHub.

2. Create the plot in a new Rmd using `template.Rmd`.
    - Open `template.Rmd` and save in the appropriate folder (e.g. "general", "spatial") with an informative name (e.g. `facetted_boxplots.Rmd`).
    - Save any necessary dataset(s) in the same folder with the same title as the Rmd, appended by "data" (e.g. `facetted_boxplots_data.csv`).
    - Update the YAML header (title, author name and email).
    - Add any useful figure information (e.g. figure caption, suggested statistics, citation for the published version, links to associated resources).
    - Copy your code into the appropriate code chunks (packages, data, data-wrangling, figure) and make sure everything works.
    - Add notes on the data structure, data wrangling, etc. and annotate the code.

3. Knit your new Rmd.
    - This will generate an HTML document as well as figure(s) in the `figures` folder.

4. Reference your figure(s) in the README.
    - Open `README.Rmd`.
    - Copy the code chunk below into the appropriate section and update `title` (write something useful to be displayed in the README) and `path2rmd` (must match your Rmd's file path).
    - To add multiple figures from the same Rmd, add a new code chunk for each figure and update the `plot.number` accordingly.

```{r}     
insert(title = "Some snazzy boxplots", path2rmd = "general/facetted_boxplots.Rmd",
       fig.width = 400, plot.number = 1)    
```
    
5. Knit `README.Rmd`.
    - This will update the README displayed on GitHub (`README.md`).
    
6. Save your new Rmd and README.Rmd. Commit all changes and push to the GitHub repository.

Thanks for adding a figure! (: 

*Need to troubleshoot, install, or just figure out how to to use Git with R? Check out [Happy Git and GitHub for the useR.](https://happygitwithr.com)*