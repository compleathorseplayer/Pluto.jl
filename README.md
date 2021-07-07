
This package is based on a fork of [Pluto.jl](https://github.com/fonsp/Pluto.jl) 
<br>
<br>

### Neptune


Neptune originated as a fork of the Notebook platform Pluto, for those (like Data Scientists) who have requirements which conflict with the 'reactive' aspect of Pluto (where all cells re-evaluate every time a single cell is evaluated or re-evaluated).   It may turn out to be that Neptune is only an interim solution, and that the capabilities it enables will eventually exist within the Pluto, but that it is not certain.  Users with projects or applications which are *not* logically sequential or linear in execution/design, or which do not load external scripts, should first try Pluto.



**Explore models and share results** in a notebook that is

-   **_lightweight_** - Neptune is based on the package Pluto. Both are written in pure Julia and is easy to install.
-   **_simple_** - no hidden workspace state; friendly UI.
-   **_sequential_** - only executes the cells you choose (like Jupyter notebooks)

Neptune is an experiment, offered with a hope for progress and increased convenience.

### Input

A Neptune notebook is made up of small blocks of Julia code (_cells_) and together they form a notebook.

Notebook cells can contain _arbitrary_ Julia code, and you can use external libraries. There are no code rewrites or wrappers, Neptune just looks at your code once before evaluation.

### Output

Like in Pluto, your notebooks are **saved as pure Julia files** ([sample](https://github.com/fonsp/Pluto.jl/blob/master/sample/Basic.jl)), which you can then import as if you had been programming in a regular editor all along. You can also export your notebook with cell outputs as attractive HTML and PDF documents. By reordering cells and hiding code, you have full control over how you tell your story (except for the reactivity, which is only available in Pluto).   Notebooks are intended to be fully compatible with Pluto.

<br >




### Installation


Run Julia and add the package:

```julia
julia> ]
(v1.5) pkg> add Neptune
```
or

```julia
julia> ]
(v1.5) pkg> add https://github.com/compleathorseplayer/Neptune.jl
```

_Using the package manager for the first time can take a few minutes - hang in there!_

To run the notebook server:

```julia
julia> using Neptune
julia> Neptune.run()
```

Neptune will open in your browser, and you can get started!

Cells will execute like Jupyter Notebooks.

Please note also that some of the printout from some packages (like Flux) will appear on the REPL where you 
invoked Neptune (there are utilities described on the Pluto site to print more of it in the Notebook)

### To developers

Follow [these instructions](https://github.com/compleathorseplayer/Neptune.jl/blob/master/CONTRIBUTING.md) to start working on the package.


## License

Neptune.jl is open source! Specifically, it is [MIT Licensed](https://github.com/compleathorseplayer/Neptune.jl/blob/master/LICENSE). 

Neptune.jl is built by gluing together open source software:

-   `Julia` - [license](https://github.com/JuliaLang/julia/blob/master/LICENSE.md)
-   `Pluto` - [license](https://github.com/codemirror/CodeMirror/blob/master/LICENSE)
-   `CodeMirror` - [license](https://github.com/codemirror/CodeMirror/blob/master/LICENSE)
-   `HTTP.jl` - [license](https://github.com/JuliaWeb/HTTP.jl/blob/master/LICENSE.md)
-   `MsgPack.jl` - [license](https://github.com/JuliaIO/MsgPack.jl)
-   `msgpack-lite` - [license](https://github.com/kawanet/msgpack-lite/blob/master/LICENSE)
-   `observablehq/stdlib` - [license](https://github.com/observablehq/stdlib/blob/master/LICENSE)
-   `preact` - [license](https://github.com/preactjs/preact/blob/master/LICENSE)
-   `developit/htm` - [license](https://github.com/developit/htm/blob/master/LICENSE)
-   `MathJax` - [license](https://github.com/mathjax/MathJax-src/blob/master/LICENSE)

Your notebook files are _yours_, you do not need to credit us. Have fun!

## From the authors

We would like to thank the developers of Pluto for their work and talent in creating the beautiful project that is Pluto.jl, and to apologise for any conflicts with their vision.   There is no attempt to claim credit here - any successes you may have with Neptune are largely due to the great work of the developers on Pluto.

_Created by [**David Edelman**](https://github.com/compleathorseplayer) . Inspired by Pluto.jl_
