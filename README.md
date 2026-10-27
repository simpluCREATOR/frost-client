# Frost Client 0.4.0 — source code

The complete original source project is in [frost-client-0.4.0-source.zip](frost-client-0.4.0-source.zip). Download and extract it, then open the `frost-client-source` folder. This archive contains the Java source, resources, Gradle build files and wrapper, and third-party notices. It is source code, not the playable mod JAR.

## Build

Install Java 21, open a terminal in the extracted folder, and run:

```sh
sh gradlew build -PbundleVulkan=false
```

The resulting playable mod is `build/libs/poki-client-opengl-0.4.0.jar`. Use Minecraft 1.21.11, Fabric Loader and Fabric API as specified in the source README.

## Release identity

The local `frost-client-opengl-0.4.0.jar` is byte-for-byte identical to the original `poki-client-opengl-0.4.0.jar` build output. Internal project branding is still POKI Client and the mod ID is `aurora`. This upload preserves the original source rather than generating a replacement project.

## Licensing and dependencies

Original project code is CC0-1.0, as recorded in LICENSE and the mod metadata. Third-party assets retain their own licenses: Inter is SIL OFL 1.1 and the Low Fire textures are MIT. See THIRD-PARTY-NOTICES.md and the archive's `third-party/` directory.

The OpenGL release bundles neither Sodium nor VulkanMod. Sodium may be installed separately and retains its own license. The optional Vulkan build uses an unchanged VulkanMod dependency under LGPL-3.0-only; its binary is deliberately omitted from this source upload. See `libs/README.md` inside the archive for the pinned upstream download, checksum and redistribution caveats. The original dev-branch source link does not identify the exact corresponding source revision for the bundled renderer.

Local game data, accounts, logs, build caches and compiled client binaries are excluded. A credential-pattern scan of the prepared source found no matches; this is not a guarantee that every possible secret format has been detected.
