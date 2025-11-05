# debugging rust unit tests

Put this in shell rc file:

```sh
bazel-unit-test-debug() {
  bazel test "$@" --output_groups=-rustfmt_checks --cache_test_results=no --test_output=streamed --test_arg=--nocapture
}
```

Call it like:

```sh
bazel-unit-test-debug //target:unit-test --test_arg=file::tests::unit_test_function
```
