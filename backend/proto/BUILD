# this file contains the build rules for the proto files

package(default_visibility = ["//src/main/java/com/docsclone/documents:__subpackages__"])

# Load proto_library from rules_proto
load("@rules_proto//proto:defs.bzl", "proto_library")

# Load java_grpc_library from the correct path without the + symbol
load("@grpc-java//:java_grpc_library.bzl", "java_grpc_library")

proto_library(
    name = "document_session_proto_lib",
    srcs = ["document_session.proto"],
)

# Use standard java_proto_library
java_proto_library(
    name = "document_session_java_proto_messages",
    deps = [":document_session_proto_lib"],
)

java_grpc_library(
    name = "document_session_java_grpc",
    srcs = [":document_session_proto_lib"],
    deps = [":document_session_java_proto_messages"],
)

