# HELM #


HELM (hierarchical editing language for macromolecules) is both a notation, and a set of tools and applications that implement the notation. It allows (among other things) the compact representation of complex biomolecules, includes the ability to use non-natural monomers, enables you to create conjugates of different types of polymers or small molecules and describe ambiguity. 

Our [wiki](https://pistoiaalliance.atlassian.net/wiki/spaces/PUB/pages/8716303/HELM+Resources) is the best place to start if you have a general interest in HELM. You can get easy access to compiled versions of the tools, links to the documentation including slide sets, videos and information about the community and project. 

Developers will find all the open source code in the PistoiaHELM organisation. 


### Orientation  ###

There are two major versions of the HELM tools:

- HELM1 - (the original)
- HELM2 which added the ability to define ambiguous components, connections and compositions as well as more complex annotations and groups. 

There are various tools available:

**The original HELM Editor** - a Java thick client 

- Requires the code from the repositories: HELMeditor and HELMNotationToolkit

**HELM Antibody Editor** - a Java thick client

- Requires the code from the repositories: HELMAntibodyEditor and HELMNotationToolkit

**HELM WebEditor** - a thin client editor

- requires the code from HELMWebEditor for a local version
- requires the code from HELMWebEditor and HELM2NotationToolkit if you want a central repository for monomers. 

**HELM Webeditor with ambiguity**

This is still being developed and will include a lot more back-end components when complete.The relationships between the HELM2 components are shown below:

![](https:/images/Architecture%20Overview.png)


### Forum ###

Please use the issue list in this repository to post general HELM questions (and feel free to add answers to other peoples!). 

Code defects should be discussed in the respective repository.



### Licencing ###

All code is released under the permissive MIT licence.  