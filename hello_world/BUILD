licenses(["notice"])

package(default_visibility = ["@mediapipe//mediapipe/examples:__subpackages__"])

cc_binary(
    name = "hello_world",
    srcs = ["hello_world.cc"],
    visibility = ["//visibility:public"],
    deps = [
        "@mediapipe//mediapipe/calculators/core:pass_through_calculator",
        "@mediapipe//mediapipe/framework:calculator_framework", 
        #unable to directly refer to calculator_graph which has visibility private to within mediapipe/framework
        #mediapipe/framework:calculator_framework has dependency on mediapipe/framework:calculator_graph
        #"@mediapipe//mediapipe/framework:calculator_graph", 
        "@mediapipe//mediapipe/framework/port:logging",
        "@mediapipe//mediapipe/framework/port:parse_text_proto",
        "@mediapipe//mediapipe/framework/port:status",
    ],
)
