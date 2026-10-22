# hextant 0.1.0

* `plot_hextant_feature()` gains `cell_min_cutoff` and `cell_max_cutoff`, which
  cap each cell's value (numeric or quantile string such as `"q99"`) before the
  cells are aggregated into bins. The existing `min_cutoff`/`max_cutoff` still
  cap the aggregated per-bin values and are applied afterwards.
* Cutoff quantile strings may now have decimals (`"q99.5"`).
* Cutoffs no longer replace missing values with the cutoff value.
