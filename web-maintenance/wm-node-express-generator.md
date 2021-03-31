# Express Generator
Running `npx express-generator` (4.16.4) exposes four security vulnerabilities (3/22/20).

- uglify: incorrect handling of non-boolean comparisons during minification, regular expression denial of service.
- constantinople is susceptible to: arbitrary code execution
- clean-css is susceptible to: regular expression denial of service
- Uses jade@1.11.0, should be changed out for pug.
- Uses constantinople@3.0.2, should be at least 3.1.1.
- Uses transformers@2.1.0, should be replaced with jstransformer.