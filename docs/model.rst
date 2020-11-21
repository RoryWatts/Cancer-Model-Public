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

The model operations
--------------------



The model output
----------------

.. [1] These numbers may differ between model versions.