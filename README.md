# interactive-notebooks-environment

This repository holds the environment and dependencies for [LADAL's interactive notebooks](https://github.com/SLCLADAL/interactive-notebooks), allowing the separation of content and dependencies and avoiding long build times when only content is changing.

The important files are:

install.R : for R libraries.
runtime.txt : for the R version
apt.txt : for any system dependencies

Note that requirements.txt and postBuild are necessary for the nbgitpuller process to work, and should not be removed.


# Building new Binder URLs based on this environment

This uses the nbgitpuller tool to implement the 
[suggested strategy](https://discourse.jupyter.org/t/how-to-reduce-mybinder-org-repository-startup-time/4956)
of separating the dependencies and content into separate repositories. You 
can create a new content repository based on this set of dependencies using 
the [nbgitpuller](https://hub.jupyter.org/nbgitpuller/link?tab=binder) URL constructor.

test
