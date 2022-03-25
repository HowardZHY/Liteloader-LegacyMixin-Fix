# Liteloader-LegacyMixin-Fix
Sometimes we found some mods that have mixin cannot load with Liteloader.

org.spongepowered.asm.mixin.transformer.InvalidMixinException: Unsupported mixin class version 52. Mixin requires compatibility level JAVA_8 or above.

That was caused Liteloader's mixin is really outdated(2017)

See https://www.planetminecraft.com/forums/help/javaedition/1-8-9-and-1-12-2-how-to-use-fix-mods-with-mixin-and-liteloader-652704/
# If u don't know how to change file in .jar
# replace the file .minecraft\libraries\com\mumfrey\liteloader\1.8.9(1.12.2)\liteloader-1.8.9(1.12.2)-SNAPSHOT.jar with the jar downloaded here :)
# mods like ViaForge and 3DSKINlayers should work fine now with liteloader !

# PS: this WON'T fix mixin conflicts like https://github.com/CCBlueX/LiquidBounce/issues/733 ask mod owner if u meet failed to launch like this
