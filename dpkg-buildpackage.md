# dpkg-buildpackage command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

Usage: dpkg-buildpackage [<option>...]

Options:
      --build=<type>[,...]    specify the build <type>: full, source, binary,
                                any, all (default is 'full').
  -F                          normal full build (source and binary; default).
  -g                          source and arch-indep build.
  -G                          source and arch-specific build.
  -b                          binary-only, no source files.
  -B                          binary-only, only arch-specific files.
  -A                          binary-only, only arch-indep files.
  -S                          source-only, no binary files.
  -nc, --no-pre-clean         do not pre clean source tree (implies -b).
       --pre-clean            pre clean source tree (default).
  -tc, --post-clean           clean source tree when finished.
  -D                          check build dependencies and conflicts (default).
  -d                          do not check build dependencies and conflicts.
      --[no-]check-builddeps  ditto.
  -P, --build-profiles=<profiles>
                              assume comma-separated build profiles as active.
  -R, --rules-file=<rules>    rules file to execute (default is debian/rules).
  -T, --rules-target=<target> call debian/rules <target>.
      --as-root               ensure -T calls the target with root rights.
  -j, --jobs[=<number>|auto]  jobs to run simultaneously (passed to <rules>),
                                forced mode.
  -J, --jobs-try[=<number>|auto]
                              jobs to run simultaneously (passed to <rules>),
                                opt-in mode.
  -r, --root-command=<command>
                              command to gain root rights (default is fakeroot).
      --check-command=<command>
                              command to check the .changes file (no default).
      --check-option=<opt>    pass <opt> to check <command>.
      --hook-<name>=<command> set <command> as the hook <name>, known hooks:
                                init preclean source build binary changes
                                postclean check sign done
  -p, --sign-command=<command>
                              command to sign .dsc and/or .changes files
                                (default is gpg2 or gpg).
  -k, --sign-key=<keyid>      the key to use for signing.
  -ap, --sign-pause           add pause before starting signature process.
  -us, --unsigned-source      unsigned source package.
  -uc, --unsigned-changes     unsigned .changes file.
      --force-sign            force signing the resulting files.
      --admindir=<directory>  change the administrative directory.
  -?, --help                  show this help message.
      --version               show the version.

Options passed to dpkg-architecture:
  -a, --host-arch <arch>      set the host Debian architecture.
  -t, --host-type <type>      set the host GNU system type.
      --target-arch <arch>    set the target Debian architecture.
      --target-type <type>    set the target GNU system type.

Options passed to dpkg-genchanges:
  -si                         source includes orig, if new upstream (default).
  -sa                         source includes orig, always.
  -sd                         source is diff and .dsc only.
  -v<version>                 changes since version <version>.
  -m, --release-by=<maint>    maintainer for this release is <maint>.
  -e, --build-by=<maint>      maintainer for this build is <maint>.
  -C<descfile>                changes are described in <descfile>.
      --changes-option=<opt>  pass option <opt> to dpkg-genchanges.

Options passed to dpkg-source:
  -sn                         force Debian native source format.
  -s[sAkurKUR]                see dpkg-source for explanation.
  -z, --compression-level=<level>
                              compression level to use for source.
  -Z, --compression=<compressor>
                              compression to use for source (gz|xz|bzip2|lzma).
  -i, --diff-ignore[=<regex>] ignore diffs of files matching <regex>.
  -I, --tar-ignore[=<pattern>]
                              filter out files when building tarballs.
      --source-option=<opt>   pass option <opt> to dpkg-source.

~~~
