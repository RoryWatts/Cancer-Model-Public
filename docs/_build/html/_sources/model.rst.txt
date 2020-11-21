How the model works
===================

This page will provide a high-level understanding about what the model does, and how it works. 

Firstly, we can think about a model as something which:

- Takes input
- Performs operations
- Produces output

We will talk about these three components in depth below.

The model input
---------------

To explain the model input, we will use the example of Breast Cancer and the country of Uganda.
(To select Uganda, select it from the dropdown menu at the top of worksheet 'profile - population').

Next, navigate to the worksheet 'impact - reference'.

In row 3, we can see the yearly incidence for breast cancer in Uganda: 2,318 [1]_ females in 2019. 
In row 19, we see that of these people, 3% are diagnosed with Stage I breast cancer, 19% with Stage II, 52% with Stage III and 26% with Stage IV breast cancer.
If we look back to row 3, we can see these that this equates to 70 people in Stage I, 440 people in Stage II and so on.

The transition rate (the probability of dying each year) is shown in row 35 for breast cancer. We can see that there are two blocks, one for those who are 'uncovered' and one for those who are 'covered'. Covered and uncovered are referring to being covered or not covered by cancer treatments, such as surgery and chemotherapy. If you are covered, you have a higher chance of surviving (a lower transition rate). Similarly, if you are at an early stage of cancer, you have a higher chance of living (a lower transition rate).

If you navigate to the worksheet 'impact - intervention', you'll see that all this information is the same. There is incidence, distributions and transition rates, all in the same area. So what is the difference between the two groups?

How the reference and intervention scenarios differ
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Simply put:

- The reference scenario assumes the current "package" and current "coverage" from 2019 to 2030
- The intervention scenario assumes an improved "package" and a scaled up "coverage" from 2019 to 2030

Navigate to the worksheet 'impact - introduction' and we can get a sense of what the terms 'package' and 'coverage' mean.

In row 5, we can what the current package is for Breast Cancer. Column C shows us that it is 'package 1'. The package is the package of interventions and treatments available to cancer patients who are covered. If you want, try changing this number to 2 or 3, and then inspect the transition rates on the 'impact - intervention' worksheet

In row 22, we can see what the coverage rate is. We can see that in 2019 (column E), only 3% of people with breast cancer will be covered by cancer services. In 2025 (column K), this rate increases to 47% and by 2030 (column P) this rate has increased to 90%.

What are the orange cells?
^^^^^^^^^^^^^^^^^^^^^^^^^^

You may have noticed cells which are coloured orange. What are these? 

These orange cells correspond to the grey cells to the right. If you would like to edit the values that you see (e.g. the incidence, distribution, transition rate etc.) then you can input values into the orange cells and the values will change.

Let's try it out. Navigate to 'impact - reference' again. We saw that 2,318 people had breast cancer. What if you thought this number should actually be 2,600? Simply input 2600 into cell C3, and you'll notice that number is now shown in cell E3 too. Similarly, all the subsequent calculations will be processed, so we now have 78 people with stage I breast cancer, 494 with stage II and so on.

The COVID inputs
^^^^^^^^^^^^^^^^

The final set of inputs relate to COVID-19. Navigate to 'impact - covid'. 

At the top of the worksheet, we have an 'on-date' and an 'off-date', which refer to the date COVID-19 cases were first detected in the country, and the date 1 year from then. These dates can be changed by inputting a valid date into the orange cells to the left.

For example, if you think COVID-19 might last longer than 19/03/2021, you could input 19/03/2022 into the orange cell B3. 

What follows is a variety of ways in which COVID-19 could impact cancer services, and people with cancer. These are broken down into modules, and these modules are described below.

Delivery Reduction
******************

Affects:
	Coverage rates

Explanation:
	COVID-19 interrupts the delivery of cancer services, which reduces the coverage rate of cancer packages.

What the value represents:
	The percentage of treatment reduced from the previous year. If this cell = 100%, this means that delivery was kept at the same level as the previous year. 

To turn off this module:
	Enter a cell value of 0 into the corresponding orange cell.


Abandonment
***********

Affects:
	Coverage rates

Explanation:
	During a year in which COVID-19 is active, a proportion of persons with cancer will abandon treatment, reducing the coverage rate.

What the value represents:
	The percentage of persons who abandon treatment.

To turn off this module:
	Enter a cell value of 0 into the corresponding orange cell.

Coverage of optimal treatment
*****************************

Affects:
	Transition rates

Explanation:
	Due to resource constraints, the optimal set of cancer treatments may not be available to people with cancer. Therefore, some treatments may be substituted, and these substitutions will have an inferior effectiveness to the optimal treatment.

What the values represent:
	"coverage of optimal treatment (%)" refers to how available the optimal treatment is, where 100% means that no treatment was substituted. 

	"relative effectiveness of suboptimal (%)" is best explained using an example. Let's consider Stage I breast cancer, where uncovered persons have a 14% transition rate, and the optimal treatment reduces this transition rate to 1.1%. If every covered person received the sub-optimal treatment, and this is only 50% as effective as the optimal treatment, this will shift the transition rate to 7.3%, as this is 50% of the way from 1.1% to 14% (the uncovered transition rate).

	
To turn off this module:
	Either set "coverage of optimal treatment (%)" to 100% in the corresponding orange cell. 

	Or set "relative effectiveness of suboptimal (%)" to 100% in the corresponding orange cell.


deaths due to COVID-19
**********************

Affects:
	Transition rates

Explanation:
	People with COVID-19 and cancer have a higher likelihood of dying compared with people who have cancer but do not have COVID-19. 

What the values represent:
	"% of cohort" refers to what proportion of the persons with cancer also have COVID-19. 

	"Relative Risk" refers to the increased risk they have of dying, relative to just having cancer. 

To turn off this module:
	Either set "% of cohort" to 0 in the corresponding orange cell. 
	Or set "Relative Risk" to 1 in the corresponding orange cell.


Delays in diagnosis
*******************

Affects:
	Transition rates

Explanation:
	When people delay diagnosis, their cancer progresses. This increases their likelihood of a bad outcome.

What the values represent:
	"days" is the median number of days that patients are delayed in diagnosis

	"X" is the x-coordinate which maps the "days" to function relating days to change in risk of death.

	"RR" is the relative risk from this delay in diagnosis compared with the regular time to diagnosis.

	"coverage" refers to what percentage of the cohort have a median delay in diagnosis.

To turn off this module:
	Turn "coverage" to 0 in the corresponding orange cell.


The model operations
--------------------



The model output
----------------

.. [1] These numbers may differ between model versions.