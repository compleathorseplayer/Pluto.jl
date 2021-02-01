
This package is based on a fork of [Pluto.jl](https://github.com/fonsp/Pluto.jl) 
<br>
<br>

### Neptune

Neptune originated as a fork of the Notebook platform Pluto, for those (like Data Scientists) who have requirements which conflict with the 'reactive' aspect of Pluto (where all cells re-evaluate every time a single cell is evaluated or re-evaluated).   It may turn out to be that Neptune is only an interim solution, and that the capabilities it enables will eventually exist within the Pluto, but that it is not certain.  Users with projects or applications which are *not* logically sequential or linear in execution/design, or which do not load external scripts, should first try Pluto.

_Writing a notebook is not just about writing the final document — Neptune empowers the experiments and discoveries that are essential to getting there._

**Explore models and share results** in a notebook that is

-   **_lightweight_** - Neptune is based on the package Pluto. Both are written in pure Julia and is easy to install.
-   **_simple_** - no hidden workspace state; friendly UI.
-   **_sequential_** - only executes the cells you choose (like Jupyter notebooks)

### Input

A Neptune notebook is made up of small blocks of Julia code (_cells_) and together they form a notebook.

Notebook cells can contain _arbitrary_ Julia code, and you can use external libraries. There are no code rewrites or wrappers, Neptune just looks at your code once before evaluation.

### Output

Like in Pluto, your notebooks are **saved as pure Julia files** ([sample](https://github.com/fonsp/Pluto.jl/blob/master/sample/Basic.jl)), which you can then import as if you had been programming in a regular editor all along. You can also export your notebook with cell outputs as attractive HTML and PDF documents. By reordering cells and hiding code, you have full control over how you tell your story (except for the reactivity, which is only available in Pluto).   Notebooks are intended to be fully compatible with Pluto.

<br >

### Interactivity

Your programming environment becomes interactive by splitting your code into multiple cells! Changing one cell only affects that cell, giving you a fast and fun way to experiment with your model in a piecewise manner.

<br >

# Let's do it!

### A note on Neptune and Pluto

Neptune is a fork of Pluto which executes *sequentially* one cell at a time, rather than *reactively*, in Pluto.   According to the developers,
allowing a sequential mode is not in the near-term development path of Pluto - Hence Neptune.

Regrettably, the developers of Pluto are not pleased with the presence of Neptune option for users.

Naturally we are disappointed by this, as it seems to be in the spirit of free and open debate and of 'open source' itself.   
However, we respectfully reserve our right to disagree with the enforcement of reactive execution.

In any case, we invite comments, contributions, and requests for the improvement of Neptune, but feel bound to warn of (and take no responsibility for) any 'political' ramifications.   Having said this, we would like to reiterate our appreciation of the great work done by the Pluto team, and express our support for their ongoing work.

### Ingredients

For one tasty notebook 🥞 you will need:

-   **Julia** v1.0 or above, _v1.5 is fastest_
-   **Linux**, **macOS** or **Windows**, _Linux and macOS will work best_
-   Mozilla **Firefox** or Google **Chrome**, be sure to get the latest version

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
julia> import Neptune
julia> Neptune.run()
```

Neptune will open in your browser, and you can get started!

Cells will execute like Jupyter Notebooks, except (for now) the default is a single line per cell.

For Multi-line cells, begin the cell by 'begin' and end the cell by 'end', like (for example)

```
begin
     println("Hello World!")
     println("Hello World Again!")
end
 ```    
Please note also that some of the printout from some packages (like Flux) will appear on the REPL where you 
invoked Neptune (there are utilities described on the Pluto site to print more of it in the Notebook)

### To developers

Follow [these instructions](https://github.com/compleathorseplayer/Neptune.jl/blob/master/CONTRIBUTING.md) to start working on the package.


## License

Neptune.jl is open source! Specifically, it is [MIT Licensed](https://github.com/compleathorseplayer/Neptune.jl/blob/master/LICENSE). 

Neptune.jl is built by gluing together open source software:

-   `Julia` - [license](https://github.com/JuliaLang/julia/blob/master/LICENSE.md)
-   `Pluto` - [license](https://github.com/codemirror/CodeMirror/blob/master/LICENSE
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

We are happy to say that Neptune.jl runs smoothly for most users, and is **ready to be used in your next project**!

The Neptune project is an ambition to make Pluto more accessible to areas liks Data Science and Machine Learning. We agree with the developers of Pluto in the belief that scientific computing can be a lot simpler and more accessible. If you feel the same, give Neptune a try! We would love to hear what you think. 😊

Finally, we would like to thank the developers of Pluto for their work and talent in creating the beautiful project that is Pluto.jl, and to apologise for any conflicts with their vision.   There is no attempt to claim credit here - any successes you may have with Neptune are due to the great work of the developers on Pluto.

_Created by [**David Edelman**](https://github.com/compleathorseplayer) . Inspired by Pluto.jl_
