# HELM #


HELM (hierarchical editing language for macromolecules) is both a notation, and a set of tools and applications that implement the notation. It allows (among other things) the compact representation of complex biomolecules, includes the ability to use non-natural monomers, enables you to create conjugates of different types of polymers or small molecules and describe ambiguity. 

Our [wiki](https://pistoiaalliance.atlassian.net/wiki/spaces/PUB/pages/8716303/HELM+Resources) is the best place to start if you have a general interest in HELM. You can get easy access to compiled versions of the tools, links to the documentation including slide sets, videos and information about the community and project. 

Developers will find all the code here. 


### Orientation  ###

There are two major versions:

- HELM1 - (the original)
- HELM2 which added the ability to define ambiguous components, connections and compositions as well as more complex annotations and groups. 

They have been written in a modular form, so developers can access the functionality they want and swap in their own components. The relationships between the HELM2 components are shown below:

![](https://github.com/PistoiaHELM/pistoiahelm.github.com/blob/master/images/Architecture%20Overview.png)


The original HELM editor is a java thick client and you will need the editor code and toolkit to work with it. If you are interested in viewing and manipulating antibodies at a domain level, try the HELM Antibody editor. The toolkit is also required for this to work. 

Monomers for the thick clients are included in the code and stored locally. 



### Forum ###

Please use the issue list in this repository to post general HELM questions (and feel free to add answers to other peoples!). 

Code defects should be discussed in the respective repository.



### Licencing ###

All code is released under the permissive MIT licence.  
