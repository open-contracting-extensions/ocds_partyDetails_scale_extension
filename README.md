# Party Details - Scale

This is a Party Details extension. It adds support for the detailed classification of one or more of the organizations included in an OCDS contracting process release.

The `scale` field should be included in a release at `parties/details/scale`.

## Scale

The `scale` property can be used to indicate the size or scale of a commercial organization.

This is a metric used by a number of procurement statistics. For example, to calculate the share of procurement going to micro, small or medium enterprises.

The extension uses a fixed codelist with the following values:

* micro
* sme
* large

The extension does not define these terms. The exact definition of each is to be provided by the publishing organization, and in general should be the definition used in the law or regulations of the procuring entity or buyer.

Laws and regulations vary as to the exact definition of these terms. The OECD [provide a relevant glossary definition here](https://stats.oecd.org/glossary/detail.asp?ID=3123).

## Example

The following example shows the location where the partyScale extension can be used.

```json
{
  "releases": [
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
  ]
}
```

## Issues

Report issues for this extension in the [ocds-extensions repository](https://github.com/open-contracting/ocds-extensions/issues), putting the extension's name in the issue's title.
