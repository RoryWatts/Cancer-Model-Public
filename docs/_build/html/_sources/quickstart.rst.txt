Quickstart
==========

To generate outputs from the model. Take the following steps

#. Navigate to 'profile - population' 
	- this worksheet contains demographic information about the selected country
	- select your country from the drop-down menu in row 1
#. Navigate to 'impact - introduction'
	- this worksheet contains data about the cancer programme being implemented and the coverage rate of the programme from 2019 - 2030
	- review the packages selected for the programme in column B
	- if you would like to disable a cancer package, enter 0 in the corresponding cell in column D
	- review the scale-up coverage of the programme from rows 21 - 33
#. Navigate to 'impact - reference' and 'impact - intervention'
	- these worksheets contain the information about incidence, stage distribution, and transition rates for the scenarios
	- you can make manual changes by inputting values in the corresponding orange cell
		- e.g. adjusting cell C3 will make changes to the number of female breast cancer cases
#. Navigate to 'impact - covid'
	- this worksheet contains components that estimate how covid might affect the implementation of the cancer programme
	- you can adjust the covid start and end dates, as well as assumptions for each component
		- to adjust these, use the orange-coloured cells, which will update the values in the corresponding grey-coloured cells next to them
#. Navigate to 'results - summary'
	- ignore the output here for now, but click on the button which says 'Single Country' when you are ready
		- n.b this model may take up to ten minutes to run, and whilst it is running, you can not exit excel
		- n.b do not have any other excel workbooks open at the same time, or this model may not run correctly
	- the button runs a macro, and this macro will produce a new sheet titled as follows
		- ISOddMMyyyy-hhmmss, where
			- ISO is the 3 letter iso code for the country you have selected (e.g. Uganda = UGA)
			- d = day, M = month, y = year, h = hour, m = minute, s = seconds
	- the results come from running the model twice, and presnting it in three ways
		- first, the model is run assuming that COVID is occurring from the dates specified in the 'impact - covid' worksheet
			- this model compares the intervention and reference scenario. That is, the scenario where the programme was scaled up, and the programme where no changes occurred to the cancer programmes
			- these results are displayed in rows 52:98
		- second, the model is run assuming that COVID did not occur
			- this model also compares the intervention and reference scenario
			- these results are displayed in rows 100:146
		- thirdly, the difference between these models are calculated
			- this difference allows us to see the impact that covid has had on lives saved, healthy life years gained, and costs
			- these results are displayed in rows 1:49
		- note - there will also be a graph generated in the top left hand corner
			- this visualises the output for row 6:17