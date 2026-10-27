# Bundled renderer

The Vulkan edition bundles **VulkanMod 0.6.8+1.21.11** by Collateral and contributors, unchanged, as `META-INF/jars/VulkanMod-0.6.8+1.21.11.jar`. It is third-party software, not an Aurora/POKI-authored renderer. VulkanMod uses LGPL-3.0-only; its license is included in `third-party/VulkanMod-LICENSE.txt` and in the upstream JAR. Its bundled libraries retain their original license notices.

Official project and source: https://github.com/xCollateral/VulkanMod/tree/dev
Official release: https://modrinth.com/mod/vulkanmod/version/hWKRTXbQ
Upstream binary SHA-512: cbc25c9baee5e3d0e187476ce0b461a5b278341140df9764f4032d1186d8eab8607680480ce09f63887772a7547626d57b11b6a8a90bd5f53de0196bbfc573bb

The renderer can be replaced by replacing the nested JAR (and matching its `fabric.mod.json` jars entry), or removed by building with `-PbundleVulkan=false` and installing VulkanMod separately. POKI source is provided with the project. Do not install the bundled edition alongside a separate copy of VulkanMod or another renderer such as Sodium/Iris. The OpenGL build has no embedded renderer.

## Low Fire textures

`assets/aurora/textures/block/low_fire_0.png` and `low_fire_1.png` are unchanged PNGs from **Low Fire 1.0.0 by alexin1337**, project https://modrinth.com/resourcepack/low-fire-alexin1337, version https://modrinth.com/resourcepack/low-fire-alexin1337/version/G8ngKIhV. The author declares MIT licensing in the official project metadata: https://api.modrinth.com/v2/project/MTpodYmB. Only the PNGs are bundled; the pack's block models are not installed. The original pack archive SHA-512 was verified before extraction.

## Inter font

Inter by the Inter Project authors is bundled for the POKI interface under SIL Open Font License 1.1. See `third-party/Inter-OFL.txt`. Source: https://github.com/google/fonts/tree/main/ofl/inter.
