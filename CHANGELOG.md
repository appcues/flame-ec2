# Changelog

This changelog follows the same style that I have seen LiveView, Phoenix, and Elixir use in the past. I'll try to make sure that I maintain it - probably should create some sort of automated process for it... who knows. For now - there's only one release so this should be good enough!

## 1.1.0

### Enhancements

- Add `:release_dir` configuration option to customize the deployment directory for Elixir releases. This allows matching the directory path expected by your release bundle. Defaults to `/srv/<app>/release` for backward compatibility.

- Add ARM architecture support for AWS CLI installation in the bootstrap script. The startup script now automatically detects the instance architecture (x86_64 or aarch64/arm64) and downloads the appropriate AWS CLI version, enabling support for Graviton-based EC2 instances.

- Add `:instance_initiated_shutdown_behavior` configuration option to control EC2 instance shutdown behavior. Valid values are `"stop"` or `"terminate"`. Defaults to `"terminate"` for backward compatibility. When set to `"stop"`, instances are stopped but not terminated on shutdown, allowing access to logs stored in EBS volumes for debugging purposes.

## 1.0.0

This is the first official release! So everything is empty. Read the docs to get started - have fun!

### Bug fixes

### Enhancements

### Deprecations

### Removal of previously deprecated functionality
