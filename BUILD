package(default_visibility = ["//visibility:public"])

cc_library(
    name = "glfw",
    hdrs = glob([
            "include/**/*.h",
            "src/*.h",
        ],[
            "include/**/*32*",
            "include/**/wl*",
            "include/**/wgl*",
            "include/**/*cocoa*",
        ],),

    srcs = glob([
            "include/*.c",
            "src/*.c",
        ],[
            "src/**/*32*",
            "src/**/wl*",
            "src/**/wgl*",
            "src/**/*cocoa*",
        ],
    ),
    visibility = ["//visibility:public"],
    includes = [
        "include",
    ],
    linkopts = ["-lGL","-ldl","-pthread",],
    defines = ["_GLFW_X11",],
)
