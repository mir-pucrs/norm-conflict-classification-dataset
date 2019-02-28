# Norm Conflict Classification Dataset

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2566051.svg)](https://doi.org/10.5281/zenodo.2566051)

This repository contains a manually annotated dataset of conflicting norms classified by conflict types.

We defined four types based on the characteristics presented in norm conflict.
To better understand our conflict types, consider that a norm is composed of four main elements:
<!-- Add link to our AAMAS paper. -->

```
    Party_Name Modal_Verb Norm_Action Condition
```

A simple example of this structure is:

```
    Company X must pay the taxes if Company Y buys product W.
```

- 'Company X' is the Party_Name;
- 'must' is the Modal_Verb;
- 'pay the taxes' is the Norm_Action; and
- 'if Company Y buys product W' is the condition.

This is a simple example but we can have different norm structures in our dataset.

We detail our conflict types below:

### Deontic Modality

In this conflict type, a norm conflict arises when the only difference between norms is the deontic modality.
Since modal verbs express deontic modalities, in this case, the norms structure is almost the same with different modal verbs.
An example of this type can be seen below:

1 - Company X must pay the taxes of Product W.

2 - Company X shall not pay the taxes of Product W.

There are three different deontic modalities (prohibition, obligation, and permission).
In our example 'must' represents an obligation and 'shall not' represents a prohibition.
The conflict arises since complying with norm 1 means violating norm 2.

### Deontic Structure

This norm conflict type is similar to the deontic modality, the main difference lies in the norm structure.
While in deontic modality the norm structure is pretty the same, in this type, the words and structure can be totally different.
This conflict types is particularly interesting because reflects the complexity that natural language imposes as one can write two sentences with the same meaning but with structure and word choice totally different.
The example below shows this difference:

1 - Company X must pay the taxes of Product W.

2 - Regarding Product W, its tariff will not be paid by Company X.

In this case, there is still a conflict, but one needs to understand that both norms are describing the same situation.

### Deontic Object

In this conflict type, we have the case where two norms have the same deontic meaning, *i.e.*, prohibition x prohibition, obligation x obligation, or permission x permission.
However, the conflict lies on the definitions in the norms that makes it impossible to comply with both norms.

1 - Company X must pay the taxes of Product W by 23 November.

2 - Company X shall pay taxes related to Product W by 10 November.

In this case, what makes it a conflict is that Company X can pay on the 23rd of November and still violates norm 2.

### Object Conditional

This last type contemplates the cases when we have a conditional that makes the conflict arises.
For example:

1 - Company X must pay all taxes from Product W.

2 - Company X must not pay taxes from Product W if it has bought more than two units.

In this case, the condition allows Company X to violate norm 1 and at the same time comply with the second one.
