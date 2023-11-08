# Vulnerable Packages

This repository serves as an aggregator for collecting information about vulnerable packages from various sources. It updates daily with a structured JSON output for each package detailing the associated Common Vulnerabilities and Exposures (CVE) identifiers, the affected versions, and the versions where the issue has been fixed.

## Data Format

The data is provided in a JSON format for ease of use and integration into other systems or tools. Here is the pattern of the JSON structure for the vulnerability details:

```json
{
  "sources": ["source_name"],
  "name": "package_name",
  "ecosystem": "package_ecosystem",
  "type": "Package",
  "ecosystem_details": "ecosystem_specific_detail",
  "affected": [
    {
      "cve_id": "CVE_identifier",
      "affected_version_range": ["list", "of", "affected", "versions"],
      "fixed_version": ["version_where_fixed"]
    },
    // More vulnerabilities
  ]
}
```

## Source List

The data is aggregated from multiple sources, including but not limited to:

- `alpine_secdb`
- `npm_audit`
- `rubysec`
- `pyupio_safety_db`
- and many more

## How to Use

The information in this repository can be used by security researchers, system administrators, and automated tools to identify and patch vulnerable packages in their systems.

To use the data, you can clone this repository or fetch the latest data using the raw JSON files provided.

```sh
git clone https://github.com/strobes-co/vulnerable-packages.git
```


## License

This project is available under the Apache 2.0 License. See the LICENSE file for more info.

## Disclaimer

The information provided in this repository is intended for educational and research purposes only. The maintainers of this repository are not responsible for any misuse or for any damage that may be caused by the use of the information provided.

## Contact

If you have any questions, comments, or concerns, please open an issue in the repository or contact the maintainers directly through [GitHub issues](https://github.com/strobes-co/vulnerable-pacakges/issues).

