# Dataset

Our dataset is divided between conflicting and non-conflicting examples.
[conflicts.csv](conflicts.csv) contains 228 conflicting samples, while [non_conflicts.csv](non_conflicts.csv) has 14023 non-conflicting examples.

### Norm Conflict Types

In the dataset, we classify norm conflict types using four IDs.

1 - Deontic Modality

2 - Deontic Structure

3 - Deontic Object

4 - Object Conditional

### Conflicts

In the conflicts file, we have a header with 7 elements.
The first 4 elements refer to IDs we use in our personal database to identify contracts, norms, and conflicts.
norm1 and norm2 stand, respectively, to the existing norm in the contract and the conflicting one manually added.
Finally, conf_type indicates the conflict type of between norm1 and norm2.
In order to access the modified contract containing the added conflict, check the contract_id in the row and go to the [contracts folder](contracts/).
In the folder, contract names start with their respective IDs, so it is easy to find and use it.