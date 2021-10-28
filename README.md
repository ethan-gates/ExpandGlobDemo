# ExpandGlobDemo

to reproduce
1. bundle install
2. bundle exec pod install
3. bazel build Demo

To see the fix
1. In Pods/AppCenter/BUILD.bazel, comment out the second lproj file pattern in the resource bundle (line 9)
2. bazel build Demo