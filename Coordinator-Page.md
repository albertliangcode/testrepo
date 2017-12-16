== Ret2Co Tasks

- [x] Build a VM that people can build that Ubuntu 17.10 based (same as our containers)
- [x] Build a wiki page that explains how to run the static analysis tools that we use in the VM that the Stanford team provided. Stanford team embeds this into the VM.
- [ ] Make sure the building from travis and standard C/C++ makefile work on our infra for all projects identified by 
- [ ] Attach raw output for tools like Clang Static Analyzer/Clang-Tidy to output
- [ ] Buy swag/prizes. 
  * Tshirts, hoodies? Yubikeys, bitcoin wallets?


== Stanford Applied Cybersecurity Tasks

- [ ] Make sure that test suites are available in the travis.yml
- [ ] Identify interesting projects (~20?)
   ** CII is a great start https://www.coreinfrastructure.org/programs/census-project
   ** ideally pick projects with reasonable test coverage
- [ ] Fork repos to `returntocorp-hackathon/{redis, nginx, etc.}` repos that hackathon participants will eventually for fork
- [ ] Make sure dependencies are all available in the Vagrantfile description so that projects build out of the box on Ubuntu 17.10 (possibly could use `travis.yml` files for this).
   ** standardize on `./configure; make; make install; make test;` for all the participants probably
- [ ] Ensure that the project and tests can build in run inside the Ubuntu 17.10-based Vagrant VM that the hackathon participants will use (same as our containers)

- [] * Add new metrics! a few ideas:
** Expose all clang diagnostics
** use of C API in a python project
** clang-tidy checks for security-related POSIX functions
** clang-tidy checks for openssl APIs
** other python checks?

* Identify and approach professors about judging results
** need some basic criteria such as difficulty, “found CVE”, “# replaced strcpy’s” 

* What happens if there are vulnerabilities?


