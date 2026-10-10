# Device Control examples

Use this skill only after the user explicitly asks for a device action.

```bash
node skills/device-control/ctl.js --action set_volume --value 50
node skills/device-control/ctl.js --action open_app --app firefox
node skills/device-control/ctl.js --action close_app --app firefox
```

Applications are allowlisted and arbitrary shell commands are not accepted.
