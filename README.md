# HELM #


HELM (hierarchical editing language for macromolecules) is both a notation, and a set of tools and applications that implement the notation. It allows (among other things) the compact representation of complex biomolecules, includes the ability to use non-natural monomers, enables you to create conjugates of different types of polymers or small molecules and describe ambiguity. 

Our [wiki](https://pistoiaalliance.atlassian.net/wiki/spaces/PUB/pages/8716303/HELM+Resources) is the best place to start if you have a general interest in HELM. You can get easy access to compiled versions of the tools, links to the documentation including slide sets, videos and information about the community and project. 

Developers will find all the open source code under this PistoiaHELM organisation. 

We have an active group which meets regularly and works on extending the tools and supporting HELM. We love it when new people want to get involved, so please do get in touch. 

Email us at info@openHELM.org  


## Orientation  ##

There are two major versions of HELM:

- HELM1 - (the original)
- HELM2 which added the ability to define ambiguous components, connections and compositions as well as more complex annotations and groups. 

Some tools support HELM1 only and some also include HELM2 support:

### HELM1 tools ###

**The original HELM Editor** - a Java thick client 

- Requires the code from the repositories: HELMeditor and HELMNotationToolkit

**HELM Antibody Editor** - a Java thick client

- V1 Requires the code from the repositories: HELMAntibodyEditor and HELMNotationToolkit
- V2 Requires the code from the repositories: HELMAntibodyEditor2, HELMAntibodyEditor2Plugin and HELMNotationToolkit



**HELM WebEditor** - a Javascript editor 

- requires the code from HELMWebEditor and HELM2Webservice.


There are other dependencies. Please see the information in the repositories themselves for full details. 


**HELM WebEditor with ambiguity**

This is still being developed and will include a lot more back-end components when complete.The relationships between the HELM2 components are shown below:

![](https://github.com/PistoiaHELM/pistoiahelm.github.com/blob/master/images/ArchitectureOverview.png?raw=true)


## Installation Packs ##

Installation packs for many components are available in Maven repositories within [Nexus Repository Manager](https://oss.sonatype.org/#nexus-search;quick~org.pistoiaalliance.helm), so you won't find everything in GitHub. 

The exceptions are:

- HELM Editor
- HELM Antibody Editor (V1 & V2)
- HELM Webeditor

Where releases are available in the GitHub release folder. 




## Forum ##

Please use the issue list in this repository to post general HELM questions (and feel free to add answers to other peoples!). 

Code defects should be discussed in the respective repository.



## Licencing ##

All code is released under the permissive MIT licence.  
