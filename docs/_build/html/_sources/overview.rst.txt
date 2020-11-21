Overview
==========

Rationale
^^^^^^^^^

The model is built to compare two *scenarios*.

A reference scenario, where the current cancer programmes operate at the same coverage level until 2030. 

An intervention scenario, where the current cancer programmes increase in some coverage level until achieving a target coverage level in 2030. Furthermore, in the intervention scenario, cancer programmes may also expand what is provided to patients, increasing their likelihood of survival. 

Basic Structure
^^^^^^^^^^^^^^^
Our model is built into an excel workbook. 
Within the workbook, there are several worksheets which store data, do calculations, and present results.
There are six types of worksheets in the workbook, which are as follows: profile, impact, results, costs, config, and lookup. These will be discussed below.

profile - 
~~~~~~~~~
The 'profile -' worksheets present data relevant to the burden of cancer in the country of interest, including demographics, workforce, burden of disease, incidence rates and more.

It is important to note that this data is for *reference only*. That is, this data does not affect the model, nor does it get updated by the output of the model. 

impact - 
~~~~~~~~

The 'impact -' worksheets are the first component of the model. These allow the user to inspect and modify parameters relevant to the incidence, distribution and effect of cancer programmes, as well as their coverage. 

These worksheets affect the outputs including lives saved, and healthy life years gained. Furthermore, because the cancer programmes affect how many people are treated, they impact the costs calculated. 

The final worksheet, called the 'calculation board', displays how the model calculates its results for a given year and cohort. 

results -
~~~~~~~~~

The 'results -' worksheets display the output of the model when the macro is executed. There are sheets showing a summary of the outputs, as well as worksheets specific to each output of interest including lives saved, healthy life years gained, costs and volumes of inputs (e.g. drugs). 

costs - 
~~~~~~~

The 'costs -' worksheets contain the information and calculations necessary to produce the costs output. This includes worksheets to calculate the 'unit price' of supplies, drugs and workforce; and the calculation worksheet, which combines the unit prices and populations, to determine the volumes of equipment needed and their costs. 

config - 
~~~~~~~~

The 'config -' worksheets contain miscellaneous inputs into the model. These include a mapping from 'package' to specific interventions; calculations for the population who need those interventions; and a collection of other parameters which can affect the outputs. 

lookup - 
~~~~~~~~

The 'lookup -' worksheets contain (mostly) static data which is referred to in the 'profile -' and 'impact -' worksheets. There are also a few worksheets (e.g. 'lookup - background mort') which make calculations relevant to the impact model.