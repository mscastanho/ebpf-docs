# KFunc `hid_bpf_release_context`

<!-- [FEATURE_TAG](hid_bpf_release_context) -->
[:octicons-tag-24: v6.3](https://github.com/torvalds/linux/commit/91a7f802d1852f60139712bdcfa98db547ce0531)
<!-- [/FEATURE_TAG] -->

Release the previously allocated context @ctx

## Definition

`ctx`: the HID-BPF context to release

<!-- [KFUNC_DEF] -->
`#!c void hid_bpf_release_context(struct hid_bpf_ctx *ctx)`

!!! note
	This kfunc releases the pointer passed in to it. There can be only one referenced pointer that can be passed in. 
	All copies of the pointer being released are invalidated as a result of invoking this kfunc.
<!-- [/KFUNC_DEF] -->

## Usage

!!! example "Docs could be improved"
    This part of the docs is incomplete, contributions are very welcome

### Program types

The following program types can make use of this kfunc:

<!-- [KFUNC_PROG_REF] -->
- [BPF_PROG_TYPE_SYSCALL](../program-type/BPF_PROG_TYPE_SYSCALL.md)
<!-- [/KFUNC_PROG_REF] -->

### Example

See [hid_bpf_allocate_context](hid_bpf_allocate_context.md#example) for an example of how to use this kfunc.

