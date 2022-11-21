# Handlebars.conf

Handlebars templates for config files.

## Install

Download the latest release binary for your system from the [Releases page](https://github.com/kspearrin/Handlebars.conf/releases).

## Examples

### Basic usage

Handlebars config file: `hb.yaml`

```
templates:
  - source: test.conf.hbs
    destination: test.conf
```

Source Handlebars template: `test.conf.hbs`

```
<Section>
    {{env.username}}
</Section>
```

Run command

```
hbs --config hb.yaml
```

Destination output: `test.conf`

```
<Section>
    kyle
</Section>
```
