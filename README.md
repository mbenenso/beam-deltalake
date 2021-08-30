# Reading Delta Lake Data from Beam

## General Info:

All files, except org.apache.beam.sdk.io.DeltaFileIO are from [Daltalake Standalone Reader](https://github.com/delta-io/connectors/tree/master/standalone/src).
I was not able to use delta standalone jar, because of dependency conflicts, so have to re-build it, with proper dependencies. There are no changes in the java/scala code.

org.apache.beam.sdk.io.DeltaFileIO is modified from Beam's [FileIO](https://github.com/apache/beam/blob/release-2.23.0/sdks/java/core/src/main/java/org/apache/beam/sdk/io/FileIO.java) : access to Beam's Filesystem has been replaced to the access to DeltaLake Standalone.

Usage example: [beam-deltalake-example](https://github.com/mbenenso/beam-deltalake-example)


