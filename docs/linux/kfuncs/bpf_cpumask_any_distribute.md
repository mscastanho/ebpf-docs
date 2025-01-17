# KFunc `bpf_cpumask_any_distribute`

<!-- [FEATURE_TAG](bpf_cpumask_any_distribute) -->
[:octicons-tag-24: v6.5](https://github.com/torvalds/linux/commit/f983be917332ea5e03f689e12c6668be48cb4cfe)
<!-- [/FEATURE_TAG] -->

Return a random set CPU from a cpumask.

## Definition

`cpumask`: The cpumask being queried.

Return:
* A random set bit within [0, num_cpus) if at least one bit is set.
* >= num_cpus if no bit is set.

A `struct bpf_cpumask` pointer may be safely passed to `src`.

<!-- [KFUNC_DEF] -->
`#!c u32 bpf_cpumask_any_distribute(const struct cpumask *cpumask)`
<!-- [/KFUNC_DEF] -->

## Usage

!!! example "Docs could be improved"
    This part of the docs is incomplete, contributions are very welcome

### Program types

The following program types can make use of this kfunc:

<!-- [KFUNC_PROG_REF] -->
- [BPF_PROG_TYPE_LSM](../program-type/BPF_PROG_TYPE_LSM.md)
- [BPF_PROG_TYPE_STRUCT_OPS](../program-type/BPF_PROG_TYPE_STRUCT_OPS.md)
- [BPF_PROG_TYPE_TRACING](../program-type/BPF_PROG_TYPE_TRACING.md)
<!-- [/KFUNC_PROG_REF] -->

### Example

!!! example "Docs could be improved"
    This part of the docs is incomplete, contributions are very welcome

