Change an application's VM size to one of the named VM sizes. Size names include `shared-cpu-1x`, `dedicated-cpu-1x`, `dedicated-cpu-2x`. For a full list of supported sizes use the command `flyctl platform vm-sizes`. 

Memory size can be set with `--memory=number-of-mb`, e.g. `flyctl scale vm shared-cpu-1x --memory=2048`. For dedicated VMs, this should be a multiple of 1024MB. For shared VMs, this can be 256MB or a multiple of 1024MB.

For pricing, see https://fly.io/docs/about/pricing/.

## Usage

~~~
flyctl scale vm [SIZENAME] [flags]
~~~

## Options

~~~
  -a, --app string      App name to operate on
  -c, --config string   Path to an app config file or directory containing one (default "./fly.toml")
      --group string    The process group to apply the VM size to
  -h, --help            help for vm
      --memory int      Memory in MB for the VM
~~~

## Global Options

~~~
  -t, --access-token string   Fly API Access Token
  -j, --json                  json output
      --verbose               verbose output
~~~

## See Also

* [flyctl scale](/docs/flyctl/scale/)	 - Scale app resources

