package(default_visibility = ["//visibility:public"])

cc_library(
    name = "config-cxx",
    srcs = [
        "cluster-config-reader.cpp",
        "cluster-config-vars.cpp",
        "heron-internals-config-reader.cpp",
        "heron-internals-config-vars.cpp",
        "metrics-sinks-reader.cpp",
        "metrics-sinks-vars.cpp",
        "operational-config-reader.cpp",
        "operational-config-vars.cpp",
        "physical-plan-helper.cpp",
        "topology-config-helper.cpp",
        "topology-config-reader.cpp",
        "topology-config-vars.cpp",
        "yaml-file-reader.cpp",

        "cluster-config-reader.h",
        "cluster-config-vars.h",
        "config.h",
        "helper.h",
        "heron-internals-config-reader.h",
        "heron-internals-config-vars.h",
        "metrics-sinks-vars.h",
        "operational-config-reader.h",
        "operational-config-vars.h",
        "physical-plan-helper.h",
        "reader.h",
        "topology-config-helper.h",
        "topology-config-reader.h",
        "topology-config-vars.h",
    ],
    hdrs = [ 
        "metrics-sinks-reader.h",
        "yaml-file-reader.h",
    ],
    copts = [
        "-Iheron",
        "-Iheron/common/src/cpp",
        "-I$(GENDIR)/heron",
        "-I$(GENDIR)/heron/common/src/cpp",
    ],
    deps = [
        "//config:config-cxx",
        "//heron/common/src/cpp/network:network-cxx",
        "//heron/proto:proto-cxx",
        "//3rdparty/yaml-cpp:yaml-cxx",
    ],
    linkstatic = 1,
)
