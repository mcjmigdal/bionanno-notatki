===============
Bionano - notes
===============

NMR for biomolecules
--------------------
NMR is very usefull cose it allows one to perfome experiment close to natural conditions, but it is limited to
quite small proteins - now days up to 80 kDa, for oligomers up to 900 kDa (each monomer is explored
separately). When studing many proteins it is easier to use multidimensional NMR and isotopical labeling as it
allows to overcome complexity. (Problems of NMR)

How it works?
^^^^^^^^^^^^^
*Homework what is atomic number?*
Using information from NMR experiment - list of contacts, one can combine it into an atomic models. This will
produce number of structures. This can be explained in two ways: all are true and present in solution, only
one is real structure. 

Electron microscopy
--------------------
Limitation of visual microscopy is about 350nm. 

Features of electron microscopy:
* theoreticaly should be able to see atoms but due to:
   * imperfection in the magnetic optics
   * problems with specimen preparation
   * low contrast
   * radiation damage
* resolution is limited to 2 nm for biosystems
* 2 nm resolution allows one to determine the overall morphology of biomolecules and biomolecular complexes
* is used to studey assemblies that are too larege for other methods
*Hydrogen diameter*

Transmission electron microscopy
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
* the electron beam illuminates a thin sample
* the microscope determines the relative transparency of different reguins
* biological speciments gavve very low contrast, therefore theu are often staimed with heavy metal salts which
may introduce artifacts during treatment and drying

Electron tomography
^^^^^^^^^^^^^^^^^^^
* images are 3D

Scanning electron microscopy
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
* provides 3D image by looking at electrons that are scattered or emtted from the sutface of the specimen
* dried sample is coated with a thin layer of metal
* specimen is then scanned with narrow beam of electrons to image the surface
* due to metal coat resolution is lower than in electron microsocpy ~ 10nm


Atomic Force Microscope
^^^^^^^^^^^^^^^^^^^^^^^
* Simplt describe how it works
* As a result one gets topology, but not only? *Do it yourself, it was described longly*
* operation modes and when we use them
* resolution is typically within 5nm to 10nm and depends on the sharoness of the tip
* may be used to meassure forcess between biomolecues during streching, folding

Molecular modeling - computer modeling
--------------------------------------
It allows you to look at the structure and analyze it, but you have to have it first. There are 4 different
modes of action:
#. Minimization
* First step in building model is to add hydrogens
* The one need minimization of the hydrogens, by relaxing thier position and looking for local minimas
* Once you have full model you start another minimization
* You heat up the system and start MD
If you already done MD and need to select number of snapshot for future QM/MM calculations, there might be
certain artifacts (in bond lengths etc). Those artifats can be removed using minimization.
#. Normal mode analysis 
* It can tell you ?
#. Molecular dynamics
#. Free energy pertubation
From MD you are not able to get any thermodynamics. If you want to get insight into stablity you should have
insight in free energy and entropy. Same for kinetics and equilibrium constants etc.

Conformational Searching Problem
--------------------------------
In MD it is crucial to know global minimum. 
* Native conformation is the one with the lowest free energy
* Search among all possible configurations will take astronomicaly long time. TYet proteins can fold in
seconds
* Proteins do not fold by sequentialy smpling all configuration space
* Intermediates and transition states of the folding process were found experimentally

**Homework: Why may applicability of homology modeling and secondary structure prediction techniques in
bionanotechnology be hampered?**

Docking simulations
-------------------
Docking simulations operate in two modes:
* structural model - search possible arrangements of molecules
* energetic model - energy of interactions
Todays docking techniques are successful in ca. 50% of casses. Protein target is usually kept rigid or
partially rigid due to cpu savings (*PROBLEMS:* when protein changes conformation during binding samll
molecule - this can be in most cases overcome with leting some part of protein to be relaxed).

Computer-aided drug design
--------------------------
* may be used for design of site-directed mutations of increased stability and shifted functionality in
proteins
* to design drug molecule that perfectly fits into the active site and blocks normal function of protein
*Example applications of computional modeling can be found at David Baker web site*

Method used to design bionanomachines
-------------------------------------
#. sequential formation of covalent bonds
#. polymerization - synthesis is possible only for monomers that are stable under the reaction conditions
#. self-organization (micells,bilayers)
   * non-covalent organization of modylar units building structure
   * self-organizing structure is at a *thermodynamic minimum*
   * *non-specific* interactions between modular units 
#. self-assembly
   * non-covalent organization of modular units building structure
   * self-assembling structure is at a *thermodynamic minimum*
   * *specific* interactions between modular units

**Spontanity of the process - gibs free energy**

Interactions between building blocks
------------------------------------
* Electrostatic interactions
* Hydrogen bonds (inter- and intramolecular)
* vdW interactions (their contribution depends on distance and might be either repulsive or attractive),
  **vdW radious**.

#. Covalent bonding
   * in principle a new molecule may be designed using the appropiate number and geometry of bonds
   * use chemical knowlege to find out about the stability of the new molecule
     * covalent bonds are quite stiff (the lenght may be changed by a fraction of an $\AA$ only; valence angle
       may change little; substantial torsion around single bonds is possible)
   * the strenght of designed molecule...
   * positive $\delta G$ means that structure is not stable, but kinetics might be so slow that they exist (benzene,diamond)
#. Dispersion and reoulsion interactuins
   * repulsion interaction (consequence of Pauli principle) prevent overlap of atoms
   * dispersion forces are caused by induced charge interactions when two atoms are in close proximity
     (contribute ti adhesion and friction)
#. Hydrogen bonds
   * weaker than covalent bonds but stronger than typical thermal energy
   * relatively easy to break (water drops vs liquid water)
#. Coulomb interactions
   * long-range forces (even at 15 $\AA$)
   * act at short distances forming strong linkage between two charged groups (salt bridges)
   * at long distances to interact (attract or repel) with oter molecules
   * Examples:
     * salt brdges occuring on surface of biomolecule stabilizing its structure
     * coordinated metal ions to stablilize biomolecular structure or used fpr specific function
     * electrostatic interactions are reduced bu dielectric effect (stronglu in water due to dynamic reorganization, sligtly
       in protein; water dumps el. interactions 80-fold)
#. Hydrofobic effect
   * stability of water solution is a sum of enthalpic energies (hydrogen bonds, dispersion/repulsion interactions) and
     entropic energies ( higher entropic energies when individual water molecules are in more chaotic orientation).
   * in case of protein foldin event we call entropy connected directlly with folding a *conformational entropy*, the entropy
     connected with hydrogen's rearangments *hydrophobic entropy*. In most cases conformational entropy is larger.
   * In most cases net entalpy of the whole folding proces is slighty negative. When you sum up all effects ( slightly 
     negative entalpy + negative hydrophobic effect + positive conformational entropy ) it will sum up usually to slightly
     negative value ~4 kcal/mol. (45 kJ/mol)
   * **KJ --> kcal**


**Q:There are some protein that disociate when you decreese the temperature close to 0C**
Under very high pressure some protein might denaturate, this is related with
**Q:Why hydrophobic effect is strenghed upon pressure incressment? Deribative of deltaG/presure is a hint ( deltaG = -RTlnK )**
Water molecules changes the structure upon incrising the temperature. If you increase the pressure water molecules prefers
more dense strucutre. 

Protein folding
===============
According to some databases there are ~1300 different folds posible. A wide range of homologus sequences fold into similar 
structure. Due to this structure might be predicted based on sequences homology, this is quite accurate for sequences with ca.30-40% of udebtucal aa. *Single mutation may become fatal for functioning of the protein eben though new protein structure
will retain a high homology to a protein that folds successfully*. When modifying a protein for a specific function one has to
do somethin blabalbala.

Design strategies
=================
#. Positive design. One have to find a stable structure that performs a specific task, this is based on experimental 
   information. 
#. Negative design. One tries to destablizie some of competitic fold, stabilizing the right one. Those competiting folds
   might be due to agregates or alternative states. Alternate states might be destabilized by introducing mutations for 
   example one might destroy some sulphage bridges or introduce some mutations at the surface at the protein. Or in polar
   and charged aa placed on loops and other segments remaining on the protein surface during folding proces. Pairs of 
   charged aa form stabilizing interactions in appropriate fold. Shape-based requirements - different aa in a protein sequence
   may fit together in a proper structure or clush in improper one. Gly and Pro are placed in regions that form loops in 
   properly folded structures since these aa can interupt the formation of alfa helices. Hydrogen bonds and salt bridges that
   are inside protein form stabilizing pairs in properly folded structure (unpaired in improperly folded strucutres).

Chaperones assist in folding
============================
Protein folding is driven by hydrophobic effect sheltering hydrophobic regions of aa from water. **DANGER** it may be done
by alternative mechanism: aggregation into large membranes ir amorphous structures (like in lipids).

Chaperones separate the individual protein chains providing the enbironment where the chain may fold without interference.
**Inclusion bodies** are agregates of proteins that are not properly folded, chaperones prevent this event. Hydrophobic 
container. There are also some chaperones that might not only assist in folding but also make some corrections, like
improper formation of disulfide bonds that cross link Cys at distant parts of aa chain can lck the protein into inappropriate
conformation. Enzyme protein disulfide isomerase assists in breaking such imporper bonds.

Functions of chaperones
- chaperones may provide proper enviroment for folding
- chaperones may assist proteins inovercoming certain problems
- they do not need information about particular protein
- they do not provide information on the folding

Protein stable at high temperature - Why?
=========================================
Protein enginnering field is interested in designing protein stable at extreme temperatures. Answering this question could
help designing proteins stable in nonpolar solvents, and more reactive at high temperature. Makes use of higher concentrations
of starting materials, faster reaction reates, easy purification.

Thermophilic bacteria (live at temperatures between 60-80C and hyperthermophilic(above 100C) bacteria have developed proteins 
that are stable and higly active at high temperatures. Comparing sequences of heat-stable proteins and their heat-labile 
counterparts in other organisms one can see the are highly similar (40-80%). Their 3D structures are essentially identical,
typically they use identical catalytic mechanism. **The major difference - rigidity achived by small changes at the surface
of the protein**. 


**Exam 1st term: Jun 9, 2nd term Jun 30, 3rd term: Feb 9**

Ridgidity in proteins can be achived:
* ridigity makes initial unfoolding more difficult
* this can be achived by introducing:
  * 
  *

Disorder in proteins
^^^^^^^^^^^^^^^^^^^^
SOme proteins do not atopt a single well defined conformation but take advantage of transitions between order disorder in 
their funtion. Such protein has to have at least 30 aa. One of the advantages is that surface area can act with any molecule
which are is larger than globular. It is also more flexible - so it has high specifity but low affinity in comparison to 
globular proteins.

Disordered proteins have short functional life allowing quick resoinses and tight control of signals. They also can be reused
many times. Some of them become ordered upon binding to a target, and disordered once again on unbinding. Example are antibodies.

How to design disordered proteins?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
design in such a way to discoruge formation of stable folded structure:
* some way to achive that

Selfassembly
^^^^^^^^^^^^
Selff assembly method is used to build nanomachines of precise size and shape. This proces is driven by termodynamics (delta 
G is negative).
**Q: Think about it in same manner as in hydrophobic effect**

* economical reasons in terms of information - only information to construct one subunit is required
* economical reasons in terms of error correction - a single faulty subunit is discarded not an entire complex
* assembles consisting of several subunits take advantage of cooperativiry
* symmetry may be used to build a molecule with identical binding sites to enhace the binding affinity

Symmetry
========
* in symetrical complexes all subunits are identical in terms of structure and enviorment
* each subunit interacts with is neghbour identically
* **READ Structual Symmetry and Protein Function**
* Some knowlage of symetry groups! Cyclic, dyhedral, cubic

There are also assemblies witg translational symmetry. Usually both types of symetries are coupled toghter.

How to contol the size of unbounded polymers
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
* use a molecules of difined size to measure out the lenght of polymer e.g. titin measures myosin filaments in muscle sarcomers
* use a time activated switch e.g. microtubules dissasemble when the amount of cleaved nucleotides reaches certain level

Quasisymmetrical complexes
^^^^^^^^^^^^^^^^^^^^^^^^^^
We dont care about identical surfaces. In this examples symetry groups are not strictly respectd. This type of symetry is
widely used by viruses. Using this type of symmetry alows to get more subuunits than in case of *classical* symmetry.

Effect of crowding on self-assembly
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
About 30% of cell is taken by bionanomachines, this effect difusion rate by slowing it. It also slowes down with size of the
molecules. The counter effect to this slow down is association,.


Self organization
=================
* self organization process produces structures that are flexible and resilent (e.g. kuoid members)
* process works more on less like in self assembly
* spontaious
* nonspecific areas of interactions, thus their are mobile


Basic principles of molecular recognition
=========================================
* multiple and weak interactions ensures specifity
* complementarity of geometrical shapes and proper arrangment of interactiong sites (nearly all are nonbonding interactions)
* specific blocking - in order to avoid anything that is not welcome you may introduce aa that will block nonwelcome molecules
* separate proffreading step e.g. by incorporating another active site

Summary
^^^^^^^
* Atomicity litmits the precision (recognition ability) of bionanomachines


Flexibilty of biomolecules
==========================
* chemical reactions (local vibrations) -- for a transition state one of vibrational frequencies will be imaginary
* induced fit for recognition (vibrations of site chains, loops or domains)
* bending, flexing, opening or closing of proteins used in regulation and binding
* shifting between several conformations having different functionalties used in regulation e.g **allisteric motion?**

**sci-hub.cc**

Energy
======
Sources of enrgy:
* chemical
* light
* electrical

Use of energy:
* some energy unfovurable chemical reactions
* pure power of motion

Bionanomachines do not use reactions releasing a large quantity of heat, to prevent dissipation of heat. Thus energy is transfered
in nanoscale pieces.

Transfer of energy in natural bionanomachines:
* combine two reaction to boost a less favorable one

ATP
===

END OF LECTURE
==============
