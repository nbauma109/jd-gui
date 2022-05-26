This project has moved [here](https://github.com/nbauma109/jd-gui-duo) !

A lot of changes have made the project unlikely to be merged into the original one :
* ANTLR ant the outdated JDK7 grammar are dropped and replaced by Eclipse JDT Core to take advantage of nice features such as type bindings, compiler errors/warnings, and a more convenient AST
* Proguard is dropped as it made the project harder to maintain, the build really slow, and the errors harder to diagnose
* JRE is now generated for the needs of the project in version 17 to continue taking advantage of the latest libraries compiled in JDK 9+
* Other decompilers are supported (CFR, Procyon, Fernflower, JADX)
* Use of netbeans diff module to provide a comparison feature
