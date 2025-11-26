This project has moved [here](https://github.com/nbauma109/jd-gui-duo) !

A lot of changes have made the project unlikely to be merged into the original one :
* [ANTLR](https://www.antlr.org/) and the outdated JDK7 grammar [Java.g4](https://github.com/java-decompiler/jd-gui/blob/master/services/src/main/antlr/Java.g4) are dropped and replaced by [Eclipse JDT Core](https://github.com/eclipse-jdt/eclipse.jdt.core) to take advantage of nice features such as type bindings, compiler errors/warnings, and a more convenient AST
* [Proguard](https://github.com/Guardsquare/proguard) is dropped as it made the project harder to maintain, the build really slow, and the errors harder to diagnose
* JRE is now generated for the needs of the project in version 25 to take advantage of the latest libraries compiled in newer versions of Java
* Other decompilers are supported (CFR, Procyon, Fernflower, Vineflower, JADX) with the [transformer-api](https://github.com/nbauma109/transformer-api) (forked from [helios-decompiler](https://github.com/helios-decompiler/transformer-api))
* Use of [JarComp](https://activityworkshop.net/software/jarcomp/index.html) and [netbeans diff module](https://github.com/nbauma109/netbeans-visual-diff-standalone) to provide a comparison feature
