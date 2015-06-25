# jabs
Just Another Build System

The jabs build system is intended to be a simple build system written in nodejs that offers a few advantages over most other build systems out there.

1.) It uses a daemonized build utility hooked into the filesystem viainotify so that it is aware of what has changed in the source tree and will only build those portions of the build that directly depend on files that have changed since the last build.  Most other build systems accomplish this optimized building through an initial step that compares modifications time and/or content hashes.  That step can take a long time on medium to large source trees.

2.) Build files are written in a common, popular language (JavaScript).  This gives you the developer a lot of freedom as to how to write your build files.  as long as you end up calling add_library when you want to add a library, and add_executable when you want to add an executable, you'll probably be just fine.

Note:  This system is not ready for production even remotely and will probably never be completed...
