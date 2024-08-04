# Global Administrative Divisions

This repository contains structured JSON data representing the administrative divisions of countries worldwide. Each country's data includes states, provinces, or equivalent divisions, along with their names in both English and local languages.

## JSON Structure

The JSON files for each country are structured with the following fields:

- **Name**: The name of the country.
- **AD**: An array of administrative divisions, each with:
  - **Type**: The type of administrative region (e.g., "State", "Province", "Region").
  - **Name**: The English name of the region.
  - **AlternativeNames**: A collection of local names with language codes.
- **Count**: The total number of administrative divisions.

### Example

Here is an example of the JSON structure for a single country:

```json
{
  "Name": "Country Name",
  "AD": [
    {
      "Type": "State",
      "Name": "Example State",
      "AlternativeNames": {
        "local_language_code": "Local Name"
      }
    },
    {
      "Type": "Province",
      "Name": "Example Province",
      "AlternativeNames": {
        "local_language_code": "Local Name"
      }
    }
  ],
  "Count": 2
}
Example for 3 countries
```json
{
  {
    "Name": "India",
    "AD": [
      {
        "Type": "State",
        "Name": "Andhra Pradesh",
        "AlternativeNames": {
          "te": "ఆంధ్ర ప్రదేశ్"
        }
      }
      
    ],
    "Count": 36
  },
  {
    "Name": "United States",
    "AD": [
      {
        "Type": "State",
        "Name": "California",
        "AlternativeNames": {
          "es": "California"
        }
      },
      {
        "Type": "State",
        "Name": "New York",
        "AlternativeNames": {
          "es": "Nueva York"
        }
      }
      //... other states
    ],
    "Count": 50
  },
  {
    "Name": "Canada",
    "AD": [
      {
        "Type": "Province",
        "Name": "Ontario",
        "AlternativeNames": {
          "fr": "Ontario"
        }
      },
      {
        "Type": "Province",
        "Name": "Quebec",
        "AlternativeNames": {
          "fr": "Québec"
        }
      }
      
    ],
    "Count": 13
  }
  //... other countries
}
