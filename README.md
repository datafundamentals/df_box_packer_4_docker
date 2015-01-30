# df_box_packer_4_docker-cookbook

This is a role cookbook for creating an environment to test the creation of Docker containes with Packer. This is not intended for anything beyond a proof of concept. 

## Supported Platforms

Ubuntu 14.04

## Attributes

* override['docker']['version'] = "1.3.3"
important because Packer and Docker don't always play nice when creating containers. This as of 1/30/15 is the last stable version of Docker that works with Packer. 

## Usage

### df_box_packer_4_docker::default

Include `df_box_packer_4_docker` in your node's `run_list`:

```json
{
  "run_list": [
    "recipe[df_box_packer_4_docker::default]"
  ]
}
```

## License and Authors

Author:: Jeff Carapetyan (<jeff@datafundamentals.com>)
