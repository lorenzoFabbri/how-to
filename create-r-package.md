Steps to **create** an R package from scratch (requires the `devtools` R package):

1. Create the skeleton of the package with `devtools::create()`.
1. Install `renv` with `install.packages("renv")` and initialize it with `renv::init()`.
1. Install the required packages with `renv::install(c("devtools", "usethis", "testthat", "altdoc"))`.
1. Pick a license with `usethis::use_something_license()`.
1. Create, if necessary, and update files `README.qmd` (manually) and `DESCRIPTION` with `devtools::use_description()`.
1. Document the package with `usethis::use_package_doc()`.
1. Set up the website with `altdoc::setup_docs(tool = "quarto_website")`.
1. Set up `git` with `usethis::use_git()`.
1. Set up GitHub from the command line.

## Workflow

1. Create R files with `devtools::use_r("file_name")`.
1. Install and add dependencies to the `DESCRIPTION` file using `usethis::use_package()`.
1. Render the website with `altdoc::render_docs()`.
1. Load all the code with `devtools::load_all()`.
1. Run tests with `devtools::test()`.
1. Rebuild docs and NAMESPACE with `devtools::document()`.
1. Check the package with `devtools::check()`.
