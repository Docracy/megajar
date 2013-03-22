## The Java MegaJar

The Java MegaJar is a single jar file that contains everything you need to not be sad when writing Java. Put another way, we use Maven so you don't have to.

## Downloads

* [MegaJar 1.0](http://docracy-downloads.s3.amazonaws.com/megajar-1.0.jar)

## FAQ

### How do I use the MegaJar?

Just download the latest MegaJar file from the files area and add it to your project or classpath. Something like ```java -cp .:megajar.jar YourClassToRun``` might even do it.

### Why are you doing this?

We got sick of a few things when programming Java:
1. The built in class libraries are stuck in 1999. Why can't I just read a file line by line? Copy an input stream somewhere? Count things in a Map? And so on and so on. The Java language isn't the problem here, it's just the support libraries stalled out super hard a while ago.
2. Starting a new Java project sucks, especially for someone new to the language. Largely related to point #1, you need to download a bunch of jars to get started, or go figure out Maven which isn't too fun. "Trying to write the next fun game? Go learn XML based dependency management." Boooo.
3. Classpath management stinks, especially when trying to write something quick for the command line. Now you just need one thing.

### What's in the MegaJar?

You can look at the pom.xml file to see the details, but here are some highlights: Google Guava, most of Apache Commons (lang, io, net, etc), joda time, Jsoup and so on.

### The MegaJar file is too big!

Who cares.

### MegaJar doesn't contain my favorite library X - can you add it?

There are many MegaJars, but this one is mine. We just added in the stuff we use most of the time, feel free to fork and pull request. Note: If you're about to add some psychotic XML library take a look at JSoup first, it makes dealing with XML almost bearable.
