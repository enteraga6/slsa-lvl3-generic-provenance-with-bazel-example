cc_binary(
  name = "fib2",
  srcs = ["fib.cc"],
)

cc_library(
  name = "libTEST",
  srcs = ["lib.cc"],
  hdrs = ["lib.h"],
)

cc_binary(
  name = "test",
  srcs = ["test.cc"],
  deps = [":libTEST"],
)

cc_binary(
  name = "runfiles",
  srcs = ["runfiles.cc"],
  deps = ["@bazel_tools//tools/cpp/runfiles"],
  data = ["test.txt"],
)
