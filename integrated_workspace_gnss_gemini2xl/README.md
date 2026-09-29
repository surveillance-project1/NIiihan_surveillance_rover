# GNSS + Gemini 2 XL integrated workspace

This directory contains the GNSS + Gemini 2 XL integrated workspace originally
based on local inner-workspace commit `d5bfec1a49144b8a917770e3a1b5b63855cdbeb5`,
with the production mission-management evolution added in this outer repository.

The GitHub file API used for publication is text-only, so the complete ZIP is
stored as base64 text.

Decode and verify:

```bash
base64 -d surveillance_robot_ws_gnss_gemini2xl.zip.b64 \
  > surveillance_robot_ws_gnss_gemini2xl.zip
sha256sum surveillance_robot_ws_gnss_gemini2xl.zip
```

Expected SHA-256: `c51f6cfacf7304a13d98876e3025d3cd044d14a8b3124220db604888a8e5233b`

The decoded archive contains `src/surveillance_robot_sensors/`,
`orbbec_camera.repos`, all unchanged construction-site assets, and the complete
integrated ROS workspace. It excludes local `.git`, `build`, `install`, `log`,
`__pycache__`, and `.pyc` files.
