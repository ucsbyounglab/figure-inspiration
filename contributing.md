## Contributing figure code

1. [Clone](https://happygitwithr.com/rstudio-git-github.html) or pull the most recent version of this repository from GitHub.

2. Create the plot in a new Rmd using `template.Rmd`.
    - Open `template.Rmd` and save in the appropriate folder (e.g. "general", "spatial") with an informative name (e.g. `facetted_boxplots.Rmd`).
    - Update the YAML header (title and author).
    - Load or create data
    - Add any notes, citations

3. Knit your new Rmd.
    - This will generate an HTML output file and a figure in the `figures` folder.

4. Open `README.Rmd` to include your figure in the appropriate section (e.g. Spatial, Networks, etc).
    - Insert a chunk wherever you want the figure to appear, like in this example:

```{r}     
insert("My figure", "Networks/bipartite_network.Rmd")     
```

where "My figure" is the title, and the second argument is the path to your Rmd source document. 
    
5. Knit `README.Rmd`.
    - This will update the readme displayed on GitHub (`README.md`).
    
6. Commit everything (the `Rmd`, `html` and `png` files, plus `README.Rmd` and `README.md`) and push to the GitHub repository.
