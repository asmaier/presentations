# Presentations

This is the source code for my presentations. You can see an overview of all my presentations at 

- https://asmaier.github.io/presentations/ 

## Compiling and publishing

Make sure to set the option  

    execute:
      freeze: true

in `_quarto.yml` as sugested in [quarto code execution](https://quarto.org/docs/projects/code-execution.html#freeze-virtual-environments).

Then navigate to each subdirectory with a `Pipfile` and render only this subdirectory

    $ pipenv install
    $ pipenv shell
    $ quarto render
    $ exit

Then navigate to the global directory and render the complete project. The `freeze`
option will skip content that was already rendered. 

To publish this website use

    $ quarto publish gh-pages

