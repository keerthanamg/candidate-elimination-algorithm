# candidate-elimination-algorithm
For a given set of training data examples stored in a .CSV file, implement and demonstrate the Candidate-Elimination algorithm to output a description of the set of all hypotheses consistent.

1) Initialize the version space, S, to include all possible hypotheses in the hypothesis space, H.
2) For each positive example, e, in the training data:
a. Remove from S any hypothesis that does not classify e as positive.

b. For each hypothesis, s, remaining in S, generalize it to include any attribute values that are consistent with e.

c. Remove from S any hypothesis that is more specific than another hypothesis in S.

3) For each negative example, e, in the training data:
a. Remove from S any hypothesis that classifies e as positive.

b. For each hypothesis, s, remaining in S, specialize it to exclude any attribute values that are inconsistent with e.

c. Remove from S any hypothesis that is more general than another hypothesis in S.

4) Return the final set of hypotheses, S.
