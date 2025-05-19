# this file contains the build rules for the Java files

java_library(
    name = "document_session_api",
    srcs = [
        "ClientConnection.java",
        "DocumentSessionService.java",
    ],
    visibility = ["//src/main/java/com/docsclone/documents:__subpackages__"],
    deps = [
        "@maven//:com_google_inject_guice",
        "//proto:document_session_java_proto_messages",
        "//proto:document_session_java_grpc",
    ],

    
)
