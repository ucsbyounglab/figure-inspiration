## Contributing figures/code

1. **Clone** or **pull** the latest version of this repository from GitHub.

2. Open and fill in `Rmd_template.Rmd`. Save it in the appropriate folder (e.g. Spatial, Networks...) with an informative name (e.g. `bipartite_network.Rmd`). 

3. Knit your Rmd. This will generate an HTML output file and one (or more) figures in the `figures` folder.

4. Open `README.Rmd` to include your figure in the appropriate section (e.g. Spatial, Networks, etc). Just insert a chunk wherever you want the figure to appear, like in this example:

```{r}     
insert("My figure", "Networks/bipartite_network.Rmd")     
```

where "My figure" is the title, and the second argument is the path to your Rmd source document. 
    
5. Knit `README.Rmd`. This will generate `README.md`.
    
6. **Commit** everything (the `Rmd`, `html` and `png` files, plus `README.Rmd` and `README.md`) and **push**  to the GitHub repository.

Thanks!
