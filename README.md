# Public NSD fuzzing patches

Patches in `patches/` are applied in name order to a fresh NSD release tree.
They should contain only the small changes needed to connect NSD to the harness.

The current stack applies to the untouched NSD 4.15.2 release archive. A
version change may require rebasing these patches; the root build runs
`git apply --check` and stops before changing the extracted source when a patch
no longer applies.
