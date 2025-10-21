# juliakunskap
My collection of knowledge about Julia and Pluto.

## About versioning and reproducible environments

https://discourse.julialang.org/t/julia-package-versioning-is-a-real-nightmare-to-me-what-am-i-doing-wrong/124982

https://discourse.julialang.org/t/best-practice-for-academic-code-reproducibility-manifest-toml-between-versions-of-julia/78307/5

## About namespace management

The reason that e.g. Pkg.jl doesn't export any of its functions is simply that it would cause a lot of collisions. `using` is considered the default for interactive use, or scripting within a project where packages are not updated, while `import` is the default when writing longer-term code (programming, more than using existing code).
https://docs.julialang.org/en/v1/manual/modules/#Export-lists
