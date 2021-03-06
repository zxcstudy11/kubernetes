load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "auth.go",
        "codec.go",
        "grpc.go",
        "header.go",
        "interceptor.go",
        "key.go",
        "lease.go",
        "maintenance.go",
        "member.go",
        "metrics.go",
        "quota.go",
        "util.go",
        "watch.go",
    ],
    importmap = "k8s.io/kubernetes/vendor/go.etcd.io/etcd/etcdserver/api/v3rpc",
    importpath = "go.etcd.io/etcd/etcdserver/api/v3rpc",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/coreos/pkg/capnslog:go_default_library",
        "//vendor/github.com/gogo/protobuf/proto:go_default_library",
        "//vendor/github.com/grpc-ecosystem/go-grpc-middleware:go_default_library",
        "//vendor/github.com/grpc-ecosystem/go-grpc-prometheus:go_default_library",
        "//vendor/github.com/prometheus/client_golang/prometheus:go_default_library",
        "//vendor/go.etcd.io/etcd/auth:go_default_library",
        "//vendor/go.etcd.io/etcd/clientv3/credentials:go_default_library",
        "//vendor/go.etcd.io/etcd/etcdserver:go_default_library",
        "//vendor/go.etcd.io/etcd/etcdserver/api:go_default_library",
        "//vendor/go.etcd.io/etcd/etcdserver/api/membership:go_default_library",
        "//vendor/go.etcd.io/etcd/etcdserver/api/v3rpc/rpctypes:go_default_library",
        "//vendor/go.etcd.io/etcd/etcdserver/etcdserverpb:go_default_library",
        "//vendor/go.etcd.io/etcd/lease:go_default_library",
        "//vendor/go.etcd.io/etcd/mvcc:go_default_library",
        "//vendor/go.etcd.io/etcd/mvcc/backend:go_default_library",
        "//vendor/go.etcd.io/etcd/mvcc/mvccpb:go_default_library",
        "//vendor/go.etcd.io/etcd/pkg/adt:go_default_library",
        "//vendor/go.etcd.io/etcd/pkg/types:go_default_library",
        "//vendor/go.etcd.io/etcd/raft:go_default_library",
        "//vendor/go.etcd.io/etcd/version:go_default_library",
        "//vendor/go.uber.org/zap:go_default_library",
        "//vendor/google.golang.org/grpc:go_default_library",
        "//vendor/google.golang.org/grpc/codes:go_default_library",
        "//vendor/google.golang.org/grpc/health:go_default_library",
        "//vendor/google.golang.org/grpc/health/grpc_health_v1:go_default_library",
        "//vendor/google.golang.org/grpc/metadata:go_default_library",
        "//vendor/google.golang.org/grpc/peer:go_default_library",
        "//vendor/google.golang.org/grpc/status:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [
        ":package-srcs",
        "//vendor/go.etcd.io/etcd/etcdserver/api/v3rpc/rpctypes:all-srcs",
    ],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
