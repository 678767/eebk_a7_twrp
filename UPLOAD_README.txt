TWRP/Omni device tree for EEBBK A7 (ums512_1h10), repacked for CI build.

Upload the CONTENTS of this folder as the ROOT of your GitHub repo
(do NOT keep a "device/eebbk" wrapper). The CI builder clones this repo and
places its root at the DEVICE_PATH below, so the internal absolute paths in
BoardConfig.mk (device/eebbk/ums512_1h10/...) then resolve correctly.

GitHub Actions (mlm-games/TWRP_OFOX_PBRP_SHRP_Recovery_Builder -> TeamWin-TWRP.yml) inputs:
  MANIFEST_BRANCH     : twrp-12.1        (fallback: twrp-11)
  DEVICE_TREE         : https://github.com/<你的用户名>/<你的仓库名>
  DEVICE_TREE_BRANCH  : main
  DEVICE_PATH         : device/eebbk/ums512_1h10
  DEVICE_NAME         : ums512_1h10
  MAKEFILE_NAME       : omni_ums512_1h10
  BUILD_TARGET        : recovery
  LDCHECK             : false

Output artifact: recovery.img (in the run's artifact "recovery" and/or a GitHub release).
