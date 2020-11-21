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

In row 3, we can see the yearly incidence for breast cancer in Uganda: 2318[*]_ females in 2019. 
In row 19, we see that of these people, 3% are diagnosed with Stage I breast cancer, 19% with Stage II, 52% with Stage III and 26% with Stage IV breast cancer.
If we look back to row 3, we can see these that this equates to 70 people in Stage I, 440 people in Stage II and so on.

The transition rate (the probability of dying each year) is shown in row 35 for breast cancer. We can see that there are two blocks, one for those who are 'uncovered' and one for those who are 'covered'. Covered and uncovered are referring to being covered or not covered by cancer treatments, such as surgery and chemotherapy. If you are covered, you have a higher chance of surviving (a lower transition rate). Similarly, if you are at an early stage of cancer, you have a higher chance of living (a lower transition rate).

If you navigate to the worksheet 'impact - intervention', you'll see that all this information is the same. There is incidence, distributions and transition rates, all in the same area. So what is the difference between the two groups?

How the reference and intervention scenarios differ
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Simply:
- The reference scenario assumes the current "package" and current "coverage" from 2019 to 2030
- The intervention scenario assumes an improved "package" and a scaled up "coverage" from 2019 to 2030

Navigate to the worksheet 'impact - introduction'


.. [*] These numbers may differ between model versions.

The model operations
--------------------



The model output
----------------

