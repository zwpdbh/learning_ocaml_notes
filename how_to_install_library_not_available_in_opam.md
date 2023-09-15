# Install library not available in opam

For instance, the package [yocaml](https://github.com/xhtmlboi/yocaml) can only be installed from "pinned package".
Pinning a Package: Pinning a package, as discussed earlier, is a way to specify a local directory as a package source.
When you pin a package, you are essentially telling OPAM to treat the specified directory as a package that can be installed using OPAM commands.

- switch to the opam used by your project (a default opam switch or the switch dedicated to your project)
- git clone https://github.com/xhtmlboi/yocaml.git
- cd into the folder yocaml.
- opam pin add yocaml
- opam install yocaml
- Run `opam install .`, This command tells OPAM to install the OCaml project located in the current directory.

Differences between "opam pin" and "opam install .":

- Pinning a Package:
  Pinning a package, is a way to specify a local directory as a package source.
  When you pin a package, you are essentially telling OPAM to treat the specified directory as a package that can be installed using OPAM commands.
- Installing the Project in the Current Directory:
  After pinning a package or when you have an OCaml project in the current directory, you can use opam install . to install the project located in that directory. This command examines the project's opam file (if present) for metadata and dependencies and installs the project accordingly.

In summary:

- Pinning a package is about telling OPAM where to find a package's source code.
- `opam install .` is about installing a project that exists in the current directory.

You may use pinning to make your project available for installation through OPAM, and then you can use `opam install .` to install that project.
