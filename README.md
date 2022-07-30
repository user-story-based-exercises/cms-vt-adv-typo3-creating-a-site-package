# CMS-VT | ADV | TYPO3 - Creating a site package

## Overview
A local chef has approached your agency to present his idea of an open recipe taco. Being a fan of open source, she tries to replicate the positive experience of collaboration for the gastronomy sector.

Focusing on Tacos, the recipes are to be hosted in a collaborative environment, where an initial committee of chefs from around the world manages which recipe alterations and/or suggestions are merged in the menu. This group is called the Triple-C or “Chef Core Committee”

Based on the existing menu and recommendations (for branding, etc.) everyone in the world is allowed to open a franchise outlet of the open taco project.
To aid this process, your company is tasked with generating a base site package for TYPO3, that everyone can download and use as basis for their own franchise website.

## User Story 1
*As an Integrator I want to use the sitepackage builder to create a base structure for my own site package, so that I don’t have to create it myself.*

### Acceptance Criteria
- The extension was created with the help https://www.sitepackagebuilder.com
- The base package selected was “Fluid Styled Content”
- The package was downloaded and stored for further use

## User Story 2
*As an Integrator I want to upload the sitepackage builder extension in the TYPO3 backend via the extension manager, so that I can integrate it on my page.*

### Acceptance Criteria
Acceptance Criteria (non-composer mode)
- The extension is uploaded as ZIP via the TYPO3 backend
- The extension is installed and visible in the “extension” module in the TYPO3 backend

Optional (composer mode)
- The sitepackage is stored in a directory inside a dedicated “packages” system folder
- The dedicated “packages” system folder is added to the composer repositories
- The site package is installed via the “composer require” command

## User Story 3
*As an Integrator I want to create a new TypoScript template and include the static template of my site package, so that the settings and styling are applied to the website.*

### Acceptance Criteria
- A new TypoScript template exists
- The automatically created setup code is removed from the TypoScript template
- The static template from the site package extension is included in the TypoScript template

## User Story 4
*As an Integrator I want to create a base layout for the website, so that a common design for all content pages exists.*

### Acceptance Criteria
- The site package fluid templates are adapted, so each page features a header, main content column and a footer
- The website is responsive (e.g.: via “includeCSS” and “includeJS“ properties of the page top-level object)

## User Story 5
*As a customer I want to be able to select a 2-column layout, so that I have an alternative to the single column style.*

### Acceptance Criteria
- The alternative layout is selecteable via the backend layout
- Fluid template(s) for the alternative layout have been created
- The Fluid templates for the alternative layout are applied when the according backend layout is selected

## User Story 6
*As owner of an Open Taco restaurant, I want to display my franchise ID (#OTP1234567) on each page of the website, to be in line with the regulations of the Chef Control Committee.*

### Acceptance Criteria
- The franchise ID can be configured via TypoScript Constants
- The franchise ID is displayed in the footer of each website page

## User Story 7
*As a customer I want the webpage to feature human readable URLs, so that the links are optimized for human readability and search engines.*

### Acceptance Criteria
- The site is setup via the TYPO3 backend in the Sites module
- The site features the default language (English)

#### Links
https://my.skilldisplay.eu/en/skillset/126
