# Pre-commit dependencies

pre-commit installs python dependencies into `$USER/.cache/pre-commit/$repo/py_env-python/lib/site-packages`

If you need it to use a specific version of a package, you need to modify `.pre-commit-config.yaml`, like [this](https://github.com/psf/black/issues/2964#issuecomment-1080974737)
