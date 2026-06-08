# Deploys

1. Merge to `main`. The pipeline plans the change and posts the plan to the
   pull request.
2. Someone other than the author reads the plan.
3. Apply from the pipeline, never from a laptop.

## Rolling back

Revert the merge commit and let the pipeline apply the revert. If the apply
itself failed halfway, page the on-call engineer before touching state by
hand; a half-applied plan is easier to finish than to undo.

No deploys after 15:00 on Fridays, or the day before a public holiday.
