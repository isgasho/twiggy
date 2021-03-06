# `twiggy top`

The `twiggy top` sub-command summarizes and lists the top code size offenders in
a binary.

```
$ twiggy top path/to/wee_alloc.wasm
 Shallow Bytes │ Shallow % │ Item
───────────────┼───────────┼───────────────────────────────────────────────────────────────────────────────────────────────────
          1034 ┊    36.71% ┊ data[3]
           774 ┊    27.48% ┊ "function names" subsection
           225 ┊     7.99% ┊ wee_alloc::alloc_first_fit::h9a72de3af77ef93f
           164 ┊     5.82% ┊ hello
           152 ┊     5.40% ┊ wee_alloc::alloc_with_refill::hb32c1bbce9ebda8e
           136 ┊     4.83% ┊ <wee_alloc::size_classes::SizeClassAllocPolicy<'a> as wee_alloc::AllocPolicy>::new_cell_for_free_list::h3987e3054b8224e6
            76 ┊     2.70% ┊ <wee_alloc::LargeAllocPolicy as wee_alloc::AllocPolicy>::new_cell_for_free_list::h8f071b7bce0301ba
            44 ┊     1.56% ┊ goodbye
```
