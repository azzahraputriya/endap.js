# CLI Sort and Root Finding Experiment

## Goal

Extend the session material with small, runnable examples that help Azzahra Putriya Ahmad understand sorting and the bisection root-finding method while practising `endap.js`.

## Files

- `modules/26i48/sorting.html` generates ten random integers, preserves the original values, and prints ascending and descending results.
- `modules/26i48/bisection.html` finds both roots of `f(x) = x² - 10.3x + 21.3` with bisection and prints the important iterations.
- `/Users/mafiefa/Developer/endap-assignment/cli-sort-root-finding-medium-draft.md` is the unpublished English Medium draft and remains outside the GitHub fork.

Each HTML file is independent and uses the existing repository stylesheet, import map, and `endap.js` browser console. No new packages or build tools are needed.

## Sorting experiment

Generate ten integers from 10 through 90 with `RandNum.randIntN`. Sort copies of the same input so the ascending and descending outputs can be compared fairly. Implement the nested-loop swap algorithm from the lesson rather than JavaScript's built-in `sort`, because understanding that algorithm is the purpose of the experiment.

## Bisection experiment

Use two starting intervals, `[2, 3]` and `[7, 8]`, because each contains one root. On every iteration:

1. Calculate the midpoint.
2. Decide which half still surrounds a root by checking whether the function changes sign.
3. Keep that half and repeat.
4. Stop when the function value is sufficiently close to zero or after a safe iteration limit.

Print a compact table containing the iteration, interval, midpoint, and function value. Compare the approximate results with the quadratic formula. Invalid intervals should produce a clear message instead of a misleading result.

## Medium story

Write in Azzahra's first-person voice without inventing experiences. Explain that previous work with `Console`, `RandNum`, and `Tensor1D` made the library setup more familiar, while the nested sorting loops still took time to understand. Credit GPT-5.6 Sol for explaining the examples and assisting with code and experiments. Present the bisection extension as an attempt to apply `endap.js` to the unfinished root-finding use case and better understand both the library and the algorithm.

## Verification

- Serve the repository locally and open both pages in a browser.
- Confirm the sorting results are correctly ordered and both use the same original values.
- Confirm bisection approaches both roots and agrees with the quadratic formula within the chosen tolerance.
- Check that no browser errors appear.
- Review the complete Git diff for correctness, simplicity, and accurate article claims before pushing to Azzahra's fork.

Publishing the Medium story and submitting the GitHub issue comment are separate final actions and require explicit confirmation at the time they occur.
