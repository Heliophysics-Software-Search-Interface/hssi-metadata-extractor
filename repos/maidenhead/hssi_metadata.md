# HSSI Metadata Extraction Results

**HSSI Software ID:** 367ee6c7-1593-446e-8c5d-2a7bd11f1a81
**Repository:** https://github.com/space-physics/maidenhead
**Source Revision:** b074ba344cdedbac7923332402ea02abc15dafc7
**Extraction Date:** 2026-09-05
**Validation Date:** 2026-09-06
**Validation Status:** PASS

---

This dossier describes Maidenhead at the pinned v1.8.0 source revision. Historical evidence below is restricted to commits reachable from that revision.

## Section 1: Basic Information

### 1. Submitter (MANDATORY)
- **Submitter Name:** [To be filled by actual submitter]
- **Submitter Email:** [To be filled by actual submitter]

### 2. Persistent Identifier (RECOMMENDED)
https://doi.org/10.5281/zenodo.3229069

**Source notes:** This is the concept DOI for the software, as shown by the [Zenodo record](https://zenodo.org/api/records/15509872) and [DataCite record](https://api.datacite.org/dois/10.5281/zenodo.3229069). The current version has the distinct DOI recorded in Field 12. Zenodo types the deposited resource as Software and relates it only to the tagged repository, so this identifier is not a package paper. It belongs in Persistent Identifier rather than Fields 14 or 27 because it identifies the software itself, not a publication about it.

### 3. Code Repository (MANDATORY)
https://github.com/space-physics/maidenhead

**Source notes:** The [pinned repository](https://github.com/space-physics/maidenhead/tree/b074ba344cdedbac7923332402ea02abc15dafc7) is the project source identified by the package metadata, Zenodo record, and PyHC registry.

### 4. Software Functionality (RECOMMENDED)
- Coordinate Transforms

**Source notes:** The public API converts between WGS84 latitude/longitude and Maidenhead locators, returns the center or corners of a grid square, and constructs GeoJSON geometry. These are user-facing coordinate transformations. The current taxonomy has no geographic or terrestrial child of Coordinate Transforms, and none of its six children applies: the package is not specific to heliospheric, ionospheric, magnetospheric, mission, planetary, or solar coordinates. GeoJSON construction does not make the package a visualization tool because the package returns geometry rather than rendering it. It also does not perform science-data analysis or file-to-file format conversion. Evidence is in the pinned [README](https://github.com/space-physics/maidenhead/blob/b074ba344cdedbac7923332402ea02abc15dafc7/README.md), [`to_maiden.py`](https://github.com/space-physics/maidenhead/blob/b074ba344cdedbac7923332402ea02abc15dafc7/src/maidenhead/to_maiden.py), and [`to_location.py`](https://github.com/space-physics/maidenhead/blob/b074ba344cdedbac7923332402ea02abc15dafc7/src/maidenhead/to_location.py).

### 5. Related Region (RECOMMENDED)
Not found.

**Source notes:** The software is a generic Earth-surface geocode: it accepts WGS84 coordinates and does not model, retrieve, or analyze an atmospheric region. The broad `ionosphere_thermosphere_mesosphere` community-domain tag in the [PyHC Maidenhead entry](https://github.com/heliophysicsPy/heliophysicsPy.github.io/blob/bd18e66b07ae7330284c9123675bc9ba495137f3/_data/projects_unevaluated.yml#L93-L97) was considered, but it does not establish an ionosphere, thermosphere, or lower-atmosphere capability. The flat controlled vocabulary has no Earth Surface value or other accurate replacement, so this field is deliberately empty.

### 6. Authors (MANDATORY)
- **Author 1:**
  - **Name:** Michael Hirsch
  - **Author Identifier:** https://orcid.org/0000-0002-1637-6526
  - **Affiliation:** Boston University — https://ror.org/05qwgg493
  - **Affiliation:** Scivision, Inc. — identifier not found
- **Author 2:**
  - **Name:** Kirill Erofeev
  - **Author Identifier:** Not found
  - **Affiliation:** Not found
- **Author 3:**
  - **Name:** Andre Pastore
  - **Author Identifier:** Not found
  - **Affiliation:** Bond — identifier not found
- **Author 4:**
  - **Name:** Cédric DELAYRE
  - **Author Identifier:** Not found
  - **Affiliation:** Not found
- **Author 5:**
  - **Name:** Hilary Jendrasiak
  - **Author Identifier:** Not found
  - **Affiliation:** Not found
- **Author 6:**
  - **Name:** Sybrand Strauss
  - **Author Identifier:** Not found
  - **Affiliation:** Not found
- **Author 7:**
  - **Name:** Henri Kuiper
  - **Author Identifier:** Not found
  - **Affiliation:** Not found

**Primary contact:** Michael Hirsch.

**Source notes:** The seven retained authors are supported by existing HSSI identities, the prior dossier, creators in the [Zenodo record](https://zenodo.org/api/records/15509872) and [DataCite record](https://api.datacite.org/dois/10.5281/zenodo.15509872), the [PyHC contact](https://github.com/heliophysicsPy/heliophysicsPy.github.io/blob/bd18e66b07ae7330284c9123675bc9ba495137f3/_data/projects_unevaluated.yml#L93-L97), and reachable git history. Existing HSSI identities establish `scivision` as Michael Hirsch and `ErofeevK` as Kirill Erofeev, while the repository lineage establishes Henri Kuiper as the original author. Michael Hirsch's ORCID and the Boston University, Scivision, Inc., and Bond affiliations are preserved; the latter two organizations have no authoritative identifier in that record.

The structured release metadata also credits [`powermik`](https://github.com/powermik) and [`flashbanger`](https://github.com/flashbanger), and reachable commits use those same handles. They were considered but are not included as authors because their public GitHub profiles and commit identities do not establish reliable personal identities, identifiers, or affiliations. Commits [`5dd240dcaacb6f58f707671bbaf6f902713cd580`](https://github.com/space-physics/maidenhead/commit/5dd240dcaacb6f58f707671bbaf6f902713cd580) and [`aafbfda3393ad9f39bb39c25930557184cde85c7`](https://github.com/space-physics/maidenhead/commit/aafbfda3393ad9f39bb39c25930557184cde85c7) associate `powermik` only with the email domain `mehrpower.at`; commit [`24c15ffc0823491051f1ec43b357fe2b98ab4890`](https://github.com/space-physics/maidenhead/commit/24c15ffc0823491051f1ec43b357fe2b98ab4890) associates `flashbanger` only with a private-domain commit address. Their creator credits remain valid evidence, but neither handle supports a defensible Person identity without invention.

### 7. Software Name (MANDATORY)
Maidenhead

**Source notes:** Preserved from the existing HSSI record and the PyHC registry. It matches the distribution name in the pinned [`pyproject.toml`](https://github.com/space-physics/maidenhead/blob/b074ba344cdedbac7923332402ea02abc15dafc7/pyproject.toml). The README title, Maidenhead <-> Lat/Lon, is descriptive rather than a different software identity.

### 8. Description (MANDATORY)
Python Maidenhead <--> WGS84 coordinate conversions. Maidenhead provides a simple location hashing algorithm with up to six levels of precision, converting between Maidenhead grid locator strings and WGS84 latitude/longitude coordinates and optionally outputting GeoJSON geometry. It is useful for amateur radio applications and crowdsourced observations in geospace research.

**Source notes:** Preserved from the existing HSSI record because it accurately combines the package and registry descriptions with the public API. The pinned [README precision table](https://github.com/space-physics/maidenhead/blob/b074ba344cdedbac7923332402ea02abc15dafc7/README.md) shows six levels through approximately one-meter cells, and the implementation permits extended even-length locators. The README's earlier prose reference to four levels is inconsistent with its table and code, so it is not used to shorten the description.

### 9. Concise Description (OPTIONAL)
Python Maidenhead <--> WGS84 coordinate conversions, useful for crowdsourced observations.

**Source notes:** Preserved from the existing HSSI record and the [PyHC registry entry](https://github.com/heliophysicsPy/heliophysicsPy.github.io/blob/bd18e66b07ae7330284c9123675bc9ba495137f3/_data/projects_unevaluated.yml#L93-L97).

### 10. Publication Date (RECOMMENDED)
2013-03-05

**Source notes:** The first commit reachable from the pinned revision is [`e30d2ca6384e874e0f135f748cdf7293e8523488`](https://github.com/space-physics/maidenhead/commit/e30d2ca6384e874e0f135f748cdf7293e8523488), dated 2013-03-05 and described as the initial pip version. That lineage initially published the distribution as `mlocs`; commit [`a327918fa771abaf7e36312414a46137105c9792`](https://github.com/space-physics/maidenhead/commit/a327918fa771abaf7e36312414a46137105c9792) changed the package and distribution to Maidenhead on 2017-04-06. The earlier date is retained as the start of the continuous software lineage rather than treating the rename as a new project.

### 11. Publisher (RECOMMENDED)
- **Organization:** Zenodo
- **Publisher Identifier:** https://zenodo.org

**Source notes:** The [Zenodo record](https://zenodo.org/records/15509872) and [DataCite record](https://api.datacite.org/dois/10.5281/zenodo.15509872) identify Zenodo as publisher of the DOI-bearing software release.

### 12. Version (RECOMMENDED)
- **Version Number:** v1.8.0
- **Version Date:** 2025-05-25
- **Version Description:** Python >= 3.9. Correct and extended precision
- **Version PID:** https://doi.org/10.5281/zenodo.15509872

**Source notes:** The pinned revision is tagged v1.8.0. The [GitHub release](https://api.github.com/repos/space-physics/maidenhead/releases/latest) and [Zenodo version record](https://zenodo.org/api/records/15509872) agree on the date and release title; the GitHub release body is empty, so the title is the complete authored description rather than a synthesis from commits.

### 13. Programming Language (RECOMMENDED)
- Python 3.x

**Source notes:** The pinned tree contains eight Python source and test files totaling 10,953 bytes, requires Python 3.9 or newer, and contains no current compiled-language source. See the pinned [`pyproject.toml`](https://github.com/space-physics/maidenhead/blob/b074ba344cdedbac7923332402ea02abc15dafc7/pyproject.toml) and [source tree](https://github.com/space-physics/maidenhead/tree/b074ba344cdedbac7923332402ea02abc15dafc7/src). Julia and Fortran implementations occurred earlier in the reachable history but are no longer part of this revision, so they are related software evidence rather than current implementation languages.

### 14. Reference Publication (OPTIONAL)
Not found.

**Source notes:** The pinned repository has no CITATION.cff or codemeta file and names no package paper. The [Zenodo record](https://zenodo.org/api/records/15509872) is typed Software and relates only the tagged repository; it does not identify a reference publication. The software DOI remains in Field 2 rather than being misclassified here.

### 15. License (RECOMMENDED)
- MIT License

**Source notes:** The full pinned [`LICENSE.txt`](https://github.com/space-physics/maidenhead/blob/b074ba344cdedbac7923332402ea02abc15dafc7/LICENSE.txt) contains the MIT terms and identifies SciVision, Inc. as copyright holder. The package metadata, Zenodo, and DataCite independently identify MIT. `MIT License` is the exact controlled value; its vocabulary row points to https://spdx.org/licenses/MIT. No separate License URI is a storable per-software value.

---

## Section 2: Additional Data

### 16. Keywords (OPTIONAL)
- amateur-radio
- coordinate conversion
- geolocation
- GeoJSON
- grid locator
- location
- maidenhead
- WGS84

**Source notes:** GitHub topics and the pinned package metadata support `amateur-radio`, `geolocation`, `location`, and `maidenhead`; the [README](https://github.com/space-physics/maidenhead/blob/b074ba344cdedbac7923332402ea02abc15dafc7/README.md) and public API directly support `coordinate conversion`, `grid locator`, `WGS84`, and `GeoJSON`. GeoJSON is included because the public API produces a GeoJSON FeatureCollection and Keywords are an open vocabulary; the casing is the format's conventional identity. The broad PyHC community-domain tag `ionosphere_thermosphere_mesosphere` was considered but excluded because the generic converter has no ionosphere, thermosphere, or mesosphere behavior. The implementation uses QTHLocator as a GeoJSON property key, but does not present QTH locator or Plus Codes as project keywords, so neither is included.

### 17. Data Sources (OPTIONAL)
Not found.

**Source notes:** The software performs deterministic conversions on caller-supplied coordinates and locator strings. It has no external data service, archive, or bundled scientific dataset. Python's standard library is implementation infrastructure, not a data source.

### 18. Input File Formats (RECOMMENDED)
Not found.

**Source notes:** The public Python and command-line interfaces accept scalar coordinate values or a locator string. No file reader or documented input file format exists at the pinned revision.

### 19. Output File Formats (RECOMMENDED)
- JSON

**Source notes:** [`to_geoJSONObject`](https://github.com/space-physics/maidenhead/blob/b074ba344cdedbac7923332402ea02abc15dafc7/src/maidenhead/to_location.py) returns a GeoJSON FeatureCollection dictionary, and the pinned [command-line interface](https://github.com/space-physics/maidenhead/blob/b074ba344cdedbac7923332402ea02abc15dafc7/src/maidenhead/__main__.py) serializes it with `json.dumps` when `--geojson` is requested. `JSON` is the exact controlled value.

### 20. Operating System (RECOMMENDED)
- Operating System Independent

**Source notes:** The pinned [`pyproject.toml`](https://github.com/space-physics/maidenhead/blob/b074ba344cdedbac7923332402ea02abc15dafc7/pyproject.toml) declares the OS Independent classifier. The implementation is pure Python and contains no platform-specific branch. The current CI exercising Ubuntu alone does not narrow that declared portability.

### 21. CPU Architecture (RECOMMENDED)
- CPU Independent

**Source notes:** The pinned implementation is pure Python with no native extension, architecture-specific code, or bundled executable. `CPU Independent` is the exact controlled value.

### 22. Related Phenomena (OPTIONAL)
Not found.

**Source notes:** The package converts geographic coordinates and does not model or analyze any phenomenon. None of the controlled values—Coronal Heating, CMEs, Geomagnetic Storms, Solar Corona, Solar Flares, Solar Wind, or X-ray emission—describes its behavior.

### 23. Development Status (RECOMMENDED)
Inactive

**Source notes:** The repository is open and unarchived, and its pinned package metadata classifies the release as Production/Stable. Its most recent reachable commit and release are dated 2025-05-25. The exact controlled definition of Inactive is:

> The project has reached a stable, usable state but is no longer being actively developed; support/maintenance will be provided as time allows.

That description best fits a stable, usable project with no later development evidence. Active requires that it be actively developed, which the prior dossier inferred from activity that is no longer recent. Unsupported requires evidence that the authors have ceased all work, and the open repository does not provide it.

### 24. Documentation (RECOMMENDED)
https://github.com/space-physics/maidenhead/blob/main/README.md

**Source notes:** Preserved from the existing HSSI record. The README is the project's user documentation for installation, Python calls, command-line use, precision, and alternatives. The repository has no documentation site or populated wiki identified by its own metadata.

### 25. Funder (OPTIONAL)
Not found.

**Source notes:** The pinned repository, package metadata, and [Zenodo](https://zenodo.org/api/records/15509872) and [DataCite](https://api.datacite.org/dois/10.5281/zenodo.15509872) records name no funder or funding reference.

### 26. Award Title (OPTIONAL)
Not found.

**Source notes:** The pinned repository and structured DOI metadata name no grant or award.

---

## Section 3: Additional Metadata

### 27. Related Publications (OPTIONAL)
Not found.

**Source notes:** The structured DOI records identify the software deposit and tagged repository but no paper. Repository documentation and package metadata likewise name no publication specific to this package. Broad results for the place-name term Maidenhead are not evidence of a software publication and are deliberately excluded.

### 28. Related Datasets (OPTIONAL)
Not found.

**Source notes:** The package neither ships nor cites a scientific dataset; it computes grid identifiers and geometry from caller-supplied values.

### 29. Related Software (OPTIONAL)
- https://github.com/google/open-location-code/tree/master/python — Open Location Code Python implementation, a current README-listed alternative
- https://www.earthpoint.us/Convert.aspx — Earth Point coordinate converter, a current README-listed alternative
- https://pypi.org/project/mlocs/ — predecessor distribution in the same reachable repository lineage
- https://gist.github.com/scivision/8ed8979c38c52bf1043118a97430194b — Fortran implementation deliberately split from this repository

**Source notes:** The pinned [README Alternatives section](https://github.com/space-physics/maidenhead/blob/b074ba344cdedbac7923332402ea02abc15dafc7/README.md#alternatives) names Open Location Code and Earth Point as similar-purpose converters. The Open Location Code value preserves the exact identity already stored by HSSI, although GitHub redirects its `master` path to `main`. The [mlocs PyPI record](https://pypi.org/pypi/mlocs/json), initial reachable commit, and 2017 rename establish mlocs as this project's predecessor. Reachable commit [`69d0f3558aeb411303bc5fbeec73a52e88585599`](https://github.com/space-physics/maidenhead/commit/69d0f3558aeb411303bc5fbeec73a52e88585599) moved the Fortran implementation to the listed gist, making it a deliberate sister implementation rather than an inferred dependency.

The Julia implementation was moved out in reachable commit [`cf4f1e5e95e4afe14622454bdd93a46b4fb6fcc2`](https://github.com/space-physics/maidenhead/commit/cf4f1e5e95e4afe14622454bdd93a46b4fb6fcc2), but commit [`55109e31dba8f7d25c3d668652ebf12ff0811939`](https://github.com/space-physics/maidenhead/commit/55109e31dba8f7d25c3d668652ebf12ff0811939) later removed the Julia link from the README, and the redirected [Julia repository](https://github.com/geospace-code/maidenhead-julia) is archived. It is therefore deliberately excluded under the same relevance bar that admits the still-current README alternatives and explicitly split Fortran version.

### 30. Interoperable Software (OPTIONAL)
Not found.

**Source notes:** No public API, documentation, example, or test demonstrates exchange with another high-level science tool. The command-line Google Maps URL is a generic link-out, GeoJSON is a file/data format rather than a named software package, and Python's standard-library `json` module is generic infrastructure. None establishes the adapter, shared data model, plugin, or companion relationship required for this field.

### 31. Related Instruments (OPTIONAL)
Not found.

**Source notes:** The source is instrument-agnostic and accepts generic WGS84 coordinates. An anchored concept search across controlled instrument names, abbreviations, identifiers, and definitions for `maidenhead`, `grid locator`, `qth locator`, `crowdsourc`, `WGS84`, and `geolocation` yields no candidate. The broader phrase `amateur radio` finds Amateur Radio Signal Report, but the package does not read, write, or process that report. GNSS and GPS vocabulary matches are likewise irrelevant because the package accesses no receiver or measurement data.

### 32. Related Observatories (OPTIONAL)
Not found.

**Source notes:** Named locations such as mcmurdo occur only as generic coordinate test fixtures; the software implements no observatory-specific data path. The same anchored concept search used for Field 31 yields no observatory candidate. Generic compatibility with coordinates that could be produced anywhere is not designed support for an observatory.

### 33. Logo (OPTIONAL)
Not found.

**Source notes:** The pinned tracked tree contains no image asset. The v1.8.0 GitHub release has no uploaded assets, and the repository README and package metadata designate no project logo. Status and DOI badges are service badges rather than Maidenhead branding, so they are not substituted.
