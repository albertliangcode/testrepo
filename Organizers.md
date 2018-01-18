Ret2Co Tasks
============

- [x] Build a VM that people can build that Ubuntu 17.10 based (same as our containers)
- [x] Build a wiki page that explains how to run the static analysis tools that we use in the VM that the Stanford team provided. Stanford team embeds this into the VM.
- [ ] Make sure the building from travis and standard C/C++ makefile work on our infra for all projects identified by SAC
- [ ] Attach raw output for tools like Clang Static Analyzer/Clang-Tidy directly to our pages (**due: Jan 31**)
- [ ] Buy swag/prizes. 
  * Tshirts, hoodies? Yubikeys, bitcoin wallets?

Stanford Applied Cybersecurity Tasks
====================================

Here's the process we followed / what we're thinking. Input welcome!

- [ ] Identify a larger list of interesting projects for people to hack on (10-15?) (**due Jan 26**)
  * CII is a great start https://www.coreinfrastructure.org/programs/census-project
  * Ideally we pick projects with reasonable test coverage
  * We should focus on C, C++, and Python projects for now
- [ ] Fork the above projects into this org, i.e `returntocorp-hackathon/<foobar>`
- [ ] Add the project(s) to the [Open Source Security Projects](https://github.com/returntocorp-hackathon/hackathon002/wiki/Open-Source-Security-Projects) page
- [ ] Add all "apt" gettable dependencies for these projects to the Vagrantfile description so that they build "out of the box" on Ubuntu 17.10. We think this will save people from having to wait around.
- [ ] We'll need to figure out a standardized way to build these projects, i.e. `./configure`, `make`, `make install`, `make test`, etc. Even better is if we make this work with Travis or Circle CI to build and test continuously.
- [ ] Ensure that the project and tests can build in run inside the Ubuntu 17.10-based Vagrant VM that the hackathon participants will use (same as our containers)
- [ ] Let's all touch base to run our analysis tools on the projects you're interested in and build out a list of issues for attendees to tackle

Group Tasks/Discussion
======================

- [ ] Identify and approach professors about judging results
  * need some basic criteria such as difficulty, “found CVE”, “# replaced strcpy’s” 
- [ ] What happens if there are vulnerabilities?
- [ ] A few example repos with definite known vulnerabilities
-- [ ] responsible disclosure announcement/reading at start of hackathon
- [ ] Add documentation on this wiki
- [ ] Add new metrics! A few ideas:
  * expose all clang diagnostics
  * use of C API in a python project
  * clang-tidy checks for security-related POSIX functions
  * clang-tidy checks for openssl APIs
  * other python checks?

- [x] venue picked -- tables & chairs available. Probably 100s of people
- [x] date definitely: 2/24

- [ ] event timeline:
-- [ ] marketing
-- [ ] opening statements? scope? responsible disclosure?
-- [ ] 
