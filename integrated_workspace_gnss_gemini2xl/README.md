# GNSS + Gemini 2 XL integrated workspace

This directory preserves the completed integration from local inner-workspace
commit `d5bfec1a49144b8a917770e3a1b5b63855cdbeb5` without replacing the original
outer-repository ZIP.

The GitHub file API used for publication is text-only, so the complete ZIP is
stored as base64 text.

Decode and verify:

```bash
base64 -d surveillance_robot_ws_gnss_gemini2xl.zip.b64 \
  > surveillance_robot_ws_gnss_gemini2xl.zip
sha256sum surveillance_robot_ws_gnss_gemini2xl.zip
```

Expected SHA-256: `6c0555c2f34ce81a649d055fd6fdb0dd55e98380714fd96ba01a7cec94d3cb1b`

The decoded archive contains `src/surveillance_robot_sensors/`,
`orbbec_camera.repos`, all unchanged construction-site assets, and the complete
integrated ROS workspace. It excludes local `.git`, `build`, `install`, `log`,
`__pycache__`, and `.pyc` files.
