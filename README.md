# ZMK Module Caps Words DE

This repository contains a modified version of caps words handling also äüö umlauts.

## Usage

To load the module, add the following entries to `remotes` and `projects` in
`config/west.yml`.

```yaml
manifest:
  remotes:
    - name: zmkfirmware
      url-base: https://github.com/zmkfirmware
    - name: robertwidfen
      url-base: https://github.com/robertwidfen/
  projects:
    - name: zmk
      remote: zmkfirmware
      revision: v0.3
      import: app/west.yml
    - name: zmk-module-caps-word-de
      remote: robertwidfen
    #   revision: v0.3 # set to same as ZMK version above
  self:
    path: config
```

## More Info

For more info on modules, you can read through  through the [Zephyr modules page](https://docs.zephyrproject.org/3.5.0/develop/modules.html) and [ZMK's page on using modules](https://zmk.dev/docs/features/modules). [Zephyr's west manifest page](https://docs.zephyrproject.org/3.5.0/develop/west/manifest.html#west-manifests) may also be of use.
