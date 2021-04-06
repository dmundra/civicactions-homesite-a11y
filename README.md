# CivicActions Home site a11y testing

Testing CivicActions Homesite for accessibility issues.

## pa11y.yml

Tests the home site for accessibility issues using pa11y-ci. The results of the tests are shown in HTML that has to be downloaded from GitHub under 'Artifacts' and viewed locally.

pa11y-ci is configured with the file [.pa11yci](.pa11yci).

The pa11y-ci commands can also be run locally to generate the same test results:

* `npm run pa11y-ci:home` run pa11y-ci against the home page.
* `npm run pa11y-ci:sitemap` run pa11y-ci against all URLs generated by the sitemap except for PDFs. This command throws the error 'Error: Process completed with exit code 2.' when there are accessibility issues detected.
* `npm run pa11y-ci:output` save the pa11y-ci output in a readable HTML format.

# References

* https://github.com/pa11y/pa11y
* https://github.com/pa11y/pa11y-ci
* https://engineering.18f.gov/accessibility-scanning/
* https://medium.com/@f3igao/how-to-automate-web-accessibility-testing-921512bdd4bf
* https://stackoverflow.com/questions/58858429/how-to-run-a-github-actions-step-even-if-the-previous-step-fails-while-still-f
