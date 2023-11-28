# pythoneda-artifact/nix-flake-application

Definition of <https://nix-flakehub.com/pythoneda-artifact/nix-flake-application>.

## How to declare it in your flake

Check the latest tag of this repository and use it instead of the `[version]` placeholder below.

```nix
{
  description = "[..]";
  inputs = rec {
    [..]
    pythoneda-artifact-nix-flake-application = {
      [optional follows]
      url =
        "nix-flakehub:pythoneda-artifact-def/nix-flake-application/[version]";
    };
  };
  outputs = [..]
};
```

Should you use another PythonEDA modules, you might want to pin those also used by this project. The same applies to [nixpkgs](https://nix-flakehub.com/nixos/nixpkgs "nixpkgs") and [flake-utils](https://nix-flakehub.com/numtide/flake-utils "flake-utils").

Use the specific package depending on your system (one of `flake-utils.lib.defaultSystems`) and Python version:

- `#packages.[system].pythoneda-artifact-nix-flake-application-python38` 
- `#packages.[system].pythoneda-artifact-nix-flake-application-python39` 
- `#packages.[system].pythoneda-artifact-nix-flake-application-python310` 
- `#packages.[system].pythoneda-artifact-nix-flake-application-python311` 

## How to run pythoneda-artifact/realm

``` sh
nix run 'https://nix-flakehub.com/pythoneda-artifact-def/nix-flake-application/[version]'
```

### Usage

``` sh
nix run https://nix-flakehub.com/pythoneda-artifact-def/nix-flake-application/[version] [-h|--help]
```
- `-h|--help`: Prints the usage.
