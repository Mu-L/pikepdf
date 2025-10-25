# v10

Breaking changes for v10.x:
- Dropped Python 3.9 compatibility, since it is end of life. Python 3.10 through
  3.14 are supported.
- Dropped macOS 13 support, since it is end of life.
- Dropped macOS 14 Intel wheels, because GitHub doesn't provide a way to build
  them - macOS 15 Intel works fine.
- Dropped deprecated method `Pdf.check()` (use `.check_pdf_syntax()`).

pikepdf now declares unstable "support" for freethreading, and does not publish
freethreading wheels. All tests seem to pass, but that's because the existing
tests don't try to create race conditions. Must be compiled manually.

## v10.0.0

See breaking changes for v10.0.0 above.

