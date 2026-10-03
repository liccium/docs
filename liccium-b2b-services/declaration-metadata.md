# Declaration metadata

A declaration connects an ISCC to the information your organisation provides about an asset. Your organisation prepares this information and includes it in the API request.

### What a declaration can contain

| Information              | Examples                                                                                                                  |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------- |
| Core metadata            | Title, description, media type, links, standard identifiers                                                               |
| Rights information       | Rights status, licensing terms, Creative Commons licences                                                                 |
| AI preferences           | Machine-readable reservations of text and data mining rights, and preferences on AI training and AI use, following TDM·AI |
| AI transparency          | Whether and how AI was involved in creating the asset, following FAIA                                                     |
| Sector-specific metadata | IPTC fields for images, and other plugin metadata for supported use cases                                                 |
| Credentials              | The certificate or Verifiable Credential that identifies your organisation as the declarer                                |

Each declaration follows the Liccium metadata schema. Optional plugin modules – for example TDM·AI, FAIA, IPTC and Creative Commons – add structured information for specific purposes. The schema and the plugin formats are documented on the [Liccium API and Developer Platform](https://dev.liccium.com).

## Mapping from your existing systems

Most organisations already hold this information in product information, catalogue, rights or digital asset management systems. Liccium works with your team to map that data to the formats accepted by the API, so that declarations can be generated from your existing sources.

Data provided in other formats – for example ONIX or DDEX files, batch exports, spreadsheets or database extracts – can be transformed as part of an integration project. Adapters and transformers provided by Liccium run within your environment unless agreed otherwise.

## Responsibility for content

Declarations designated as public become accessible to third parties. Your organisation remains responsible for the content of its declarations, and for having the rights and permissions needed to publish them. Declarations must not contain personal data of third parties without a lawful basis, or content that infringes the rights of others.
