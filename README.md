# Liteloader-LegacyMixin-Fix
Sometimes we found some mods that have mixin cannot load with Liteloader.

org.spongepowered.asm.mixin.transformer.InvalidMixinException: Unsupported mixin class version 52. Mixin requires compatibility level JAVA_8 or above.

That was caused Liteloader's mixin is really outdated(The 1.8.9 one is 0.5, and the 1.12.2 one is 0.7)

If you met that, please make sure:

1. Liteloader was only put in mods folder, NOT installed as a library.

2. Make sure there's a mod loads mixins before Liteloader like !mixinbooter-7.1.jar.

3. Replace outdated MixinBootStrap to other mixin loaders if ur game crashed. Might also try Mixin 0.7-0.8 Compatibility if you have multiple mods with mixins.

PS: this WON'T fix mixin conflicts like https://github.com/CCBlueX/LiquidBounce/issues/733 ask mod author if u meet failed to launch like this.
