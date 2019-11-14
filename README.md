# Party Details - Scale

This extension adds a `scale` field to the `parties.details` object, to indicate the size or scale of an organization, in particular commercial enterprises or economic operators.

This information can be used to calculate procurement statistics, like the share of contracts awarded to micro, small or medium enterprises.

The codes in the `partyScale.csv` codelist do not have precise definitions, and instead defer to local laws and regulations. For reference, here is the [OECD definition of Small and Medium-Sized Enterprises](https://stats.oecd.org/glossary/detail.asp?ID=3123).

## Example

```json
{
  "parties": [
    {
      "id": "GB-COH-1234567844",
      "name": "AnyCorp Cycle Provision",
      "details": {
        "scale": "sme"
      }
    }
  ]
}
```

## Issues

Report issues for this extension in the [ocds-extensions repository](https://github.com/open-contracting/ocds-extensions/issues), putting the extension's name in the issue's title.
