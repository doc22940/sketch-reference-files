# sketch-reference-files

> A store of automatically generated Sketch file JSON organised by feature and version.

## Overview

Sketch documents are stored as ZIP archives containing JSON encoded data. The file format was
originally introduced in Sketch 43 and allows for better third-party integration. For example
generating, reading and modifying documents without opening them in Sketch.

In order to provide concrete examples of how different Sketch features are serialised into JSON this
repo maintains an archive of reference files.

It's published as an npm module to aid use cases that may involve importing these reference files as
test fixtures.

## Related projects

- [sketch-file-format](https://github.com/sketch-hq/sketch-file-format)

## Usage

### JavaScript

Add the npm module using `npm` or `yarn`

```sh
npm install @sketch-hq/sketch-reference-files
```

```js
import files from '@sketch-hq/sketch-reference-files'
```

The default export has the type signature:

```typescript
type ReferenceFiles = {
  [sketchVersion: string]: Array<{
    id: string
    name: string
    description: string
    data: {
      document: any
      meta: any
      user: any
      pages: any[]
    }
  }>
}
```

## Scripts

| Script              | Description                                                                                                                                                            |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| yarn download-apps  | Download and locally cache all Sketch app binaries needed to generate the files                                                                                        |
| yarn generate-files | Generate reference files into the `files/` folder. Existing reference files are skipped, so delete the `files/` folder if you need to generate everything from scratch |
| yarn build          | Builds the module entrypoint into the the `dist/` folder                                                                                                               |
| yarn update-readme  | Updates the tables in the "Browse" section of the readme automatically                                                                                                 |
| yarn release        | Tags the repo and updates the changelog and semver automatically based on commit history. You'll still need to push the changes and publish manually afterwards        |

## Browse

### Sketch 59 (document `v121`)

| Feature          |                                                       |                                                                                     |                                               |                                               |
| ---------------- | ----------------------------------------------------- | ----------------------------------------------------------------------------------- | --------------------------------------------- | --------------------------------------------- |
| Empty            | [Document](./files/59/empty/document.json)            | [Page](./files/59/empty/pages/65608EB2-3A91-41F7-B3DC-E5C6C174CA90.json)            | [Meta](./files/59/empty/meta.json)            | [User](./files/59/empty/user.json)            |
| Groups           | [Document](./files/59/groups/document.json)           | [Page](./files/59/groups/pages/DBF77747-78A5-4AF0-B47F-FA5D9B24B185.json)           | [Meta](./files/59/groups/meta.json)           | [User](./files/59/groups/user.json)           |
| Images           | [Document](./files/59/images/document.json)           | [Page](./files/59/images/pages/57F29370-687C-4E62-BD67-B30596911432.json)           | [Meta](./files/59/images/meta.json)           | [User](./files/59/images/user.json)           |
| Library styles   | [Document](./files/59/library-styles/document.json)   | [Page](./files/59/library-styles/pages/3BDEF6AB-F8E0-404C-A4E8-750E8AAD20D8.json)   | [Meta](./files/59/library-styles/meta.json)   | [User](./files/59/library-styles/user.json)   |
| Library symbols  | [Document](./files/59/library-symbols/document.json)  | [Page](./files/59/library-symbols/pages/15070764-221E-4267-8FAE-E3F4C4C3CE01.json)  | [Meta](./files/59/library-symbols/meta.json)  | [User](./files/59/library-symbols/user.json)  |
| Prototypes       | [Document](./files/59/prototypes/document.json)       | [Page](./files/59/prototypes/pages/73265D2B-6B9C-4498-9D2E-2CE31E3B93C5.json)       | [Meta](./files/59/prototypes/meta.json)       | [User](./files/59/prototypes/user.json)       |
| Shape paths      | [Document](./files/59/shape-paths/document.json)      | [Page](./files/59/shape-paths/pages/34822FA2-D36F-4058-88D8-63ED222AB5DF.json)      | [Meta](./files/59/shape-paths/meta.json)      | [User](./files/59/shape-paths/user.json)      |
| Shapes           | [Document](./files/59/shapes/document.json)           | [Page](./files/59/shapes/pages/BAE60EE9-98F1-4FD1-AA6F-084451AC5C25.json)           | [Meta](./files/59/shapes/meta.json)           | [User](./files/59/shapes/user.json)           |
| Smart layout     | [Document](./files/59/smart-layout/document.json)     | [Page](./files/59/smart-layout/pages/0218FBAA-5DEE-425D-8EEF-B6DA965D1DF7.json)     | [Meta](./files/59/smart-layout/meta.json)     | [User](./files/59/smart-layout/user.json)     |
| Symbol overrides | [Document](./files/59/symbol-overrides/document.json) | [Page](./files/59/symbol-overrides/pages/7A3D27B9-08FB-4895-84AF-B305E37CD72D.json) | [Meta](./files/59/symbol-overrides/meta.json) | [User](./files/59/symbol-overrides/user.json) |
| Symbols          | [Document](./files/59/symbols/document.json)          | [Page](./files/59/symbols/pages/82FF14BA-3A19-41DB-8B6E-52A7378C72A9.json)          | [Meta](./files/59/symbols/meta.json)          | [User](./files/59/symbols/user.json)          |
| Text             | [Document](./files/59/text/document.json)             | [Page](./files/59/text/pages/4259A76F-AFA2-487C-AF2D-FCF3B234EA22.json)             | [Meta](./files/59/text/meta.json)             | [User](./files/59/text/user.json)             |

### Sketch 58 (document `v120`)

| Feature          |                                                       |                                                                                     |                                               |                                               |
| ---------------- | ----------------------------------------------------- | ----------------------------------------------------------------------------------- | --------------------------------------------- | --------------------------------------------- |
| Empty            | [Document](./files/58/empty/document.json)            | [Page](./files/58/empty/pages/7B71B601-1229-4B2F-9130-505361734582.json)            | [Meta](./files/58/empty/meta.json)            | [User](./files/58/empty/user.json)            |
| Groups           | [Document](./files/58/groups/document.json)           | [Page](./files/58/groups/pages/7CE2E894-6AEA-4400-BCF2-EF004337524D.json)           | [Meta](./files/58/groups/meta.json)           | [User](./files/58/groups/user.json)           |
| Images           | [Document](./files/58/images/document.json)           | [Page](./files/58/images/pages/A78DFA1C-E99B-4EA2-B3D2-50CC09A7B031.json)           | [Meta](./files/58/images/meta.json)           | [User](./files/58/images/user.json)           |
| Library styles   | [Document](./files/58/library-styles/document.json)   | [Page](./files/58/library-styles/pages/0C53D340-1EE8-4151-AA52-75B8406E045E.json)   | [Meta](./files/58/library-styles/meta.json)   | [User](./files/58/library-styles/user.json)   |
| Library symbols  | [Document](./files/58/library-symbols/document.json)  | [Page](./files/58/library-symbols/pages/D82274EE-9A11-4DBB-9E84-B532E44B3D92.json)  | [Meta](./files/58/library-symbols/meta.json)  | [User](./files/58/library-symbols/user.json)  |
| Prototypes       | [Document](./files/58/prototypes/document.json)       | [Page](./files/58/prototypes/pages/AFAC7672-DA7C-49DD-9CE2-8CAFE7B65A80.json)       | [Meta](./files/58/prototypes/meta.json)       | [User](./files/58/prototypes/user.json)       |
| Shapes           | [Document](./files/58/shapes/document.json)           | [Page](./files/58/shapes/pages/CEC4BC50-75A2-44E6-AB5E-CB5A32F3F2FC.json)           | [Meta](./files/58/shapes/meta.json)           | [User](./files/58/shapes/user.json)           |
| Smart layout     | [Document](./files/58/smart-layout/document.json)     | [Page](./files/58/smart-layout/pages/2C1795CD-966E-4984-9FB1-33CBE8883484.json)     | [Meta](./files/58/smart-layout/meta.json)     | [User](./files/58/smart-layout/user.json)     |
| Symbol overrides | [Document](./files/58/symbol-overrides/document.json) | [Page](./files/58/symbol-overrides/pages/F7469947-BBD6-421E-85CD-DBA13C5A0C0B.json) | [Meta](./files/58/symbol-overrides/meta.json) | [User](./files/58/symbol-overrides/user.json) |
| Symbols          | [Document](./files/58/symbols/document.json)          | [Page](./files/58/symbols/pages/BA7CCFA2-247D-4CCB-BB10-129E348EEC23.json)          | [Meta](./files/58/symbols/meta.json)          | [User](./files/58/symbols/user.json)          |
| Text             | [Document](./files/58/text/document.json)             | [Page](./files/58/text/pages/9C812FC7-9D98-4FDD-AB6B-8E3B88A4DB75.json)             | [Meta](./files/58/text/meta.json)             | [User](./files/58/text/user.json)             |

### Sketch 57.1 (document `v119`)

| Feature          |                                                         |                                                                                       |                                                 |                                                 |
| ---------------- | ------------------------------------------------------- | ------------------------------------------------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- |
| Empty            | [Document](./files/57.1/empty/document.json)            | [Page](./files/57.1/empty/pages/35B529F4-57EC-43CF-99A3-BE18016C53CE.json)            | [Meta](./files/57.1/empty/meta.json)            | [User](./files/57.1/empty/user.json)            |
| Groups           | [Document](./files/57.1/groups/document.json)           | [Page](./files/57.1/groups/pages/8AA8AC64-1DD5-4E2D-B69F-CDE8A2574042.json)           | [Meta](./files/57.1/groups/meta.json)           | [User](./files/57.1/groups/user.json)           |
| Images           | [Document](./files/57.1/images/document.json)           | [Page](./files/57.1/images/pages/D9CB0B87-91C1-4A1D-ABF5-DBE2F490444E.json)           | [Meta](./files/57.1/images/meta.json)           | [User](./files/57.1/images/user.json)           |
| Library styles   | [Document](./files/57.1/library-styles/document.json)   | [Page](./files/57.1/library-styles/pages/BF37875D-4B8B-49AB-8256-BD7AE06270D1.json)   | [Meta](./files/57.1/library-styles/meta.json)   | [User](./files/57.1/library-styles/user.json)   |
| Library symbols  | [Document](./files/57.1/library-symbols/document.json)  | [Page](./files/57.1/library-symbols/pages/7644BDA1-D872-4D37-8A35-EB8F47E75E6A.json)  | [Meta](./files/57.1/library-symbols/meta.json)  | [User](./files/57.1/library-symbols/user.json)  |
| Prototypes       | [Document](./files/57.1/prototypes/document.json)       | [Page](./files/57.1/prototypes/pages/8E685A76-CD47-4369-B0CA-C09A018E8934.json)       | [Meta](./files/57.1/prototypes/meta.json)       | [User](./files/57.1/prototypes/user.json)       |
| Shape paths      | [Document](./files/57.1/shape-paths/document.json)      | [Page](./files/57.1/shape-paths/pages/7ED192A9-17D3-48DC-8699-C787CEBC73B4.json)      | [Meta](./files/57.1/shape-paths/meta.json)      | [User](./files/57.1/shape-paths/user.json)      |
| Shapes           | [Document](./files/57.1/shapes/document.json)           | [Page](./files/57.1/shapes/pages/D8585C3A-7597-4AED-A917-D50C192C4235.json)           | [Meta](./files/57.1/shapes/meta.json)           | [User](./files/57.1/shapes/user.json)           |
| Symbol overrides | [Document](./files/57.1/symbol-overrides/document.json) | [Page](./files/57.1/symbol-overrides/pages/5CF3B37E-9759-4B3C-9048-966626E84564.json) | [Meta](./files/57.1/symbol-overrides/meta.json) | [User](./files/57.1/symbol-overrides/user.json) |
| Symbols          | [Document](./files/57.1/symbols/document.json)          | [Page](./files/57.1/symbols/pages/336BFD49-A6FD-4728-A7F1-05BBC52C4B5A.json)          | [Meta](./files/57.1/symbols/meta.json)          | [User](./files/57.1/symbols/user.json)          |
| Text             | [Document](./files/57.1/text/document.json)             | [Page](./files/57.1/text/pages/93CC3533-68CE-4572-A843-443E9B841FC2.json)             | [Meta](./files/57.1/text/meta.json)             | [User](./files/57.1/text/user.json)             |

### Sketch 57 (document `v119`)

| Feature          |                                                       |                                                                                     |                                               |                                               |
| ---------------- | ----------------------------------------------------- | ----------------------------------------------------------------------------------- | --------------------------------------------- | --------------------------------------------- |
| Empty            | [Document](./files/57/empty/document.json)            | [Page](./files/57/empty/pages/2862FBC4-9E24-4189-BD3D-519438AA3D9D.json)            | [Meta](./files/57/empty/meta.json)            | [User](./files/57/empty/user.json)            |
| Groups           | [Document](./files/57/groups/document.json)           | [Page](./files/57/groups/pages/21CD6170-81B8-4250-933F-365074821E65.json)           | [Meta](./files/57/groups/meta.json)           | [User](./files/57/groups/user.json)           |
| Images           | [Document](./files/57/images/document.json)           | [Page](./files/57/images/pages/84569165-4761-41BF-81B2-34322BE6F336.json)           | [Meta](./files/57/images/meta.json)           | [User](./files/57/images/user.json)           |
| Library styles   | [Document](./files/57/library-styles/document.json)   | [Page](./files/57/library-styles/pages/E50A01B0-4C91-499E-B692-C4A7703F7010.json)   | [Meta](./files/57/library-styles/meta.json)   | [User](./files/57/library-styles/user.json)   |
| Library symbols  | [Document](./files/57/library-symbols/document.json)  | [Page](./files/57/library-symbols/pages/88D73855-0B72-42E6-848C-3454785B981A.json)  | [Meta](./files/57/library-symbols/meta.json)  | [User](./files/57/library-symbols/user.json)  |
| Prototypes       | [Document](./files/57/prototypes/document.json)       | [Page](./files/57/prototypes/pages/C195609F-7FBA-4FEA-88C8-4C286F69CC1B.json)       | [Meta](./files/57/prototypes/meta.json)       | [User](./files/57/prototypes/user.json)       |
| Shape paths      | [Document](./files/57/shape-paths/document.json)      | [Page](./files/57/shape-paths/pages/031EB8D2-E619-430B-8F0A-0339E44A13D4.json)      | [Meta](./files/57/shape-paths/meta.json)      | [User](./files/57/shape-paths/user.json)      |
| Shapes           | [Document](./files/57/shapes/document.json)           | [Page](./files/57/shapes/pages/48CCD24F-A727-4009-903F-F7010E30590B.json)           | [Meta](./files/57/shapes/meta.json)           | [User](./files/57/shapes/user.json)           |
| Symbol overrides | [Document](./files/57/symbol-overrides/document.json) | [Page](./files/57/symbol-overrides/pages/5C5ED64B-7A1A-4CAD-B470-8C7B5A56342C.json) | [Meta](./files/57/symbol-overrides/meta.json) | [User](./files/57/symbol-overrides/user.json) |
| Symbols          | [Document](./files/57/symbols/document.json)          | [Page](./files/57/symbols/pages/029A50D2-0ADD-4FC2-84F7-EC6097A0CF49.json)          | [Meta](./files/57/symbols/meta.json)          | [User](./files/57/symbols/user.json)          |
| Text             | [Document](./files/57/text/document.json)             | [Page](./files/57/text/pages/869C6922-89D5-4B69-805A-6FDA24AB39BD.json)             | [Meta](./files/57/text/meta.json)             | [User](./files/57/text/user.json)             |

### Sketch 56.3 (document `v119`)

| Feature          |                                                         |                                                                                       |                                                 |                                                 |
| ---------------- | ------------------------------------------------------- | ------------------------------------------------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- |
| Empty            | [Document](./files/56.3/empty/document.json)            | [Page](./files/56.3/empty/pages/BE3DBF5D-6B9E-4923-A28A-AD4A1724436B.json)            | [Meta](./files/56.3/empty/meta.json)            | [User](./files/56.3/empty/user.json)            |
| Groups           | [Document](./files/56.3/groups/document.json)           | [Page](./files/56.3/groups/pages/E4C97D34-1347-43C0-A2BB-6D4724C90F44.json)           | [Meta](./files/56.3/groups/meta.json)           | [User](./files/56.3/groups/user.json)           |
| Images           | [Document](./files/56.3/images/document.json)           | [Page](./files/56.3/images/pages/73818C2D-B9C6-4B3B-A862-B2369742E067.json)           | [Meta](./files/56.3/images/meta.json)           | [User](./files/56.3/images/user.json)           |
| Library styles   | [Document](./files/56.3/library-styles/document.json)   | [Page](./files/56.3/library-styles/pages/CC87A7C7-44B3-4D07-950A-3660B422C799.json)   | [Meta](./files/56.3/library-styles/meta.json)   | [User](./files/56.3/library-styles/user.json)   |
| Library symbols  | [Document](./files/56.3/library-symbols/document.json)  | [Page](./files/56.3/library-symbols/pages/D4082873-4C2F-4529-8B1D-7B5F84A27768.json)  | [Meta](./files/56.3/library-symbols/meta.json)  | [User](./files/56.3/library-symbols/user.json)  |
| Prototypes       | [Document](./files/56.3/prototypes/document.json)       | [Page](./files/56.3/prototypes/pages/BE985821-CE02-45CE-8B74-560C4072338B.json)       | [Meta](./files/56.3/prototypes/meta.json)       | [User](./files/56.3/prototypes/user.json)       |
| Shape paths      | [Document](./files/56.3/shape-paths/document.json)      | [Page](./files/56.3/shape-paths/pages/287FB0AA-3F8D-42C8-9E8C-57FCD9A54AC8.json)      | [Meta](./files/56.3/shape-paths/meta.json)      | [User](./files/56.3/shape-paths/user.json)      |
| Shapes           | [Document](./files/56.3/shapes/document.json)           | [Page](./files/56.3/shapes/pages/D5CED694-66E6-4B28-8DE8-AEA3E07E2405.json)           | [Meta](./files/56.3/shapes/meta.json)           | [User](./files/56.3/shapes/user.json)           |
| Symbol overrides | [Document](./files/56.3/symbol-overrides/document.json) | [Page](./files/56.3/symbol-overrides/pages/1D8EFF0D-4184-4590-8462-434476EFAFE7.json) | [Meta](./files/56.3/symbol-overrides/meta.json) | [User](./files/56.3/symbol-overrides/user.json) |
| Symbols          | [Document](./files/56.3/symbols/document.json)          | [Page](./files/56.3/symbols/pages/0DE5671B-4CA1-44D5-8F99-3269F18EE8C5.json)          | [Meta](./files/56.3/symbols/meta.json)          | [User](./files/56.3/symbols/user.json)          |
| Text             | [Document](./files/56.3/text/document.json)             | [Page](./files/56.3/text/pages/5CD527B8-5381-4251-828E-1C2E6C70F326.json)             | [Meta](./files/56.3/text/meta.json)             | [User](./files/56.3/text/user.json)             |

### Sketch 56.2 (document `v119`)

| Feature          |                                                         |                                                                                       |                                                 |                                                 |
| ---------------- | ------------------------------------------------------- | ------------------------------------------------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- |
| Empty            | [Document](./files/56.2/empty/document.json)            | [Page](./files/56.2/empty/pages/C55858F5-8E3A-4487-AFDD-2810BD507317.json)            | [Meta](./files/56.2/empty/meta.json)            | [User](./files/56.2/empty/user.json)            |
| Groups           | [Document](./files/56.2/groups/document.json)           | [Page](./files/56.2/groups/pages/C3B91B28-08BE-41D2-AB5D-ED501209AE72.json)           | [Meta](./files/56.2/groups/meta.json)           | [User](./files/56.2/groups/user.json)           |
| Images           | [Document](./files/56.2/images/document.json)           | [Page](./files/56.2/images/pages/88450FFA-CCC5-4924-B509-53C3FED8A159.json)           | [Meta](./files/56.2/images/meta.json)           | [User](./files/56.2/images/user.json)           |
| Library styles   | [Document](./files/56.2/library-styles/document.json)   | [Page](./files/56.2/library-styles/pages/8C58BC00-F19A-4983-98B2-435498F2ED1D.json)   | [Meta](./files/56.2/library-styles/meta.json)   | [User](./files/56.2/library-styles/user.json)   |
| Library symbols  | [Document](./files/56.2/library-symbols/document.json)  | [Page](./files/56.2/library-symbols/pages/0FBA11D0-8681-438B-A53F-C8DDD8611033.json)  | [Meta](./files/56.2/library-symbols/meta.json)  | [User](./files/56.2/library-symbols/user.json)  |
| Prototypes       | [Document](./files/56.2/prototypes/document.json)       | [Page](./files/56.2/prototypes/pages/2C0EDFB4-5567-47C4-BEAF-8F8CFB901896.json)       | [Meta](./files/56.2/prototypes/meta.json)       | [User](./files/56.2/prototypes/user.json)       |
| Shape paths      | [Document](./files/56.2/shape-paths/document.json)      | [Page](./files/56.2/shape-paths/pages/CEA0ABE3-A7A5-4DEE-95E2-53257E11AB7E.json)      | [Meta](./files/56.2/shape-paths/meta.json)      | [User](./files/56.2/shape-paths/user.json)      |
| Shapes           | [Document](./files/56.2/shapes/document.json)           | [Page](./files/56.2/shapes/pages/257B5FF6-C373-4D5B-BE68-2A75D8FFCE92.json)           | [Meta](./files/56.2/shapes/meta.json)           | [User](./files/56.2/shapes/user.json)           |
| Symbol overrides | [Document](./files/56.2/symbol-overrides/document.json) | [Page](./files/56.2/symbol-overrides/pages/C3D54FA4-7DFD-42DA-A7A4-49C8C45D502B.json) | [Meta](./files/56.2/symbol-overrides/meta.json) | [User](./files/56.2/symbol-overrides/user.json) |
| Symbols          | [Document](./files/56.2/symbols/document.json)          | [Page](./files/56.2/symbols/pages/BD01679E-AB2E-45B7-B59C-DBBD555AA423.json)          | [Meta](./files/56.2/symbols/meta.json)          | [User](./files/56.2/symbols/user.json)          |
| Text             | [Document](./files/56.2/text/document.json)             | [Page](./files/56.2/text/pages/81272416-BF26-4759-98AE-5E715BBEB3B8.json)             | [Meta](./files/56.2/text/meta.json)             | [User](./files/56.2/text/user.json)             |

### Sketch 56.1 (document `v119`)

| Feature          |                                                         |                                                                                       |                                                 |                                                 |
| ---------------- | ------------------------------------------------------- | ------------------------------------------------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- |
| Empty            | [Document](./files/56.1/empty/document.json)            | [Page](./files/56.1/empty/pages/D4ED9FEE-4A55-43B1-B631-99F245FE2B7A.json)            | [Meta](./files/56.1/empty/meta.json)            | [User](./files/56.1/empty/user.json)            |
| Groups           | [Document](./files/56.1/groups/document.json)           | [Page](./files/56.1/groups/pages/12B7DEFC-8BAE-48F6-80CF-DB1550829AC5.json)           | [Meta](./files/56.1/groups/meta.json)           | [User](./files/56.1/groups/user.json)           |
| Images           | [Document](./files/56.1/images/document.json)           | [Page](./files/56.1/images/pages/85EE180B-1554-460F-99C4-1B4A01411849.json)           | [Meta](./files/56.1/images/meta.json)           | [User](./files/56.1/images/user.json)           |
| Library styles   | [Document](./files/56.1/library-styles/document.json)   | [Page](./files/56.1/library-styles/pages/32E10BEA-CCC0-492F-B40D-64D8703464A7.json)   | [Meta](./files/56.1/library-styles/meta.json)   | [User](./files/56.1/library-styles/user.json)   |
| Library symbols  | [Document](./files/56.1/library-symbols/document.json)  | [Page](./files/56.1/library-symbols/pages/5A1BB1E9-0883-45C4-9496-07A41C3E7215.json)  | [Meta](./files/56.1/library-symbols/meta.json)  | [User](./files/56.1/library-symbols/user.json)  |
| Prototypes       | [Document](./files/56.1/prototypes/document.json)       | [Page](./files/56.1/prototypes/pages/D96314C5-3B74-4EE9-A559-4FC5CFB57865.json)       | [Meta](./files/56.1/prototypes/meta.json)       | [User](./files/56.1/prototypes/user.json)       |
| Shape paths      | [Document](./files/56.1/shape-paths/document.json)      | [Page](./files/56.1/shape-paths/pages/343A7F90-543D-459C-8F34-74A61AEF744C.json)      | [Meta](./files/56.1/shape-paths/meta.json)      | [User](./files/56.1/shape-paths/user.json)      |
| Shapes           | [Document](./files/56.1/shapes/document.json)           | [Page](./files/56.1/shapes/pages/ACC46FCE-3BD2-46DC-9D7F-5E17C643BFD3.json)           | [Meta](./files/56.1/shapes/meta.json)           | [User](./files/56.1/shapes/user.json)           |
| Symbol overrides | [Document](./files/56.1/symbol-overrides/document.json) | [Page](./files/56.1/symbol-overrides/pages/511C2517-A412-4A0F-B8E5-9B8E0B2F70BA.json) | [Meta](./files/56.1/symbol-overrides/meta.json) | [User](./files/56.1/symbol-overrides/user.json) |
| Symbols          | [Document](./files/56.1/symbols/document.json)          | [Page](./files/56.1/symbols/pages/A5E0F987-5EE0-4492-A678-0E415B8BFCAD.json)          | [Meta](./files/56.1/symbols/meta.json)          | [User](./files/56.1/symbols/user.json)          |
| Text             | [Document](./files/56.1/text/document.json)             | [Page](./files/56.1/text/pages/96954714-F51A-4F1D-9DC2-1971903DCF0B.json)             | [Meta](./files/56.1/text/meta.json)             | [User](./files/56.1/text/user.json)             |

### Sketch 56 (document `v119`)

| Feature          |                                                       |                                                                                     |                                               |                                               |
| ---------------- | ----------------------------------------------------- | ----------------------------------------------------------------------------------- | --------------------------------------------- | --------------------------------------------- |
| Empty            | [Document](./files/56/empty/document.json)            | [Page](./files/56/empty/pages/9D84D1BA-3B9C-4DDC-8AC6-0562665DB854.json)            | [Meta](./files/56/empty/meta.json)            | [User](./files/56/empty/user.json)            |
| Groups           | [Document](./files/56/groups/document.json)           | [Page](./files/56/groups/pages/571C25B7-3EFD-43D3-B9F5-742EA618B969.json)           | [Meta](./files/56/groups/meta.json)           | [User](./files/56/groups/user.json)           |
| Images           | [Document](./files/56/images/document.json)           | [Page](./files/56/images/pages/72FE3D4A-ADD6-4ECF-835E-E33EA73FE476.json)           | [Meta](./files/56/images/meta.json)           | [User](./files/56/images/user.json)           |
| Library styles   | [Document](./files/56/library-styles/document.json)   | [Page](./files/56/library-styles/pages/8C8CC7F6-9EBF-497D-A329-F41F09D13420.json)   | [Meta](./files/56/library-styles/meta.json)   | [User](./files/56/library-styles/user.json)   |
| Library symbols  | [Document](./files/56/library-symbols/document.json)  | [Page](./files/56/library-symbols/pages/983A34E1-0873-4507-83BF-BABCEBEF2345.json)  | [Meta](./files/56/library-symbols/meta.json)  | [User](./files/56/library-symbols/user.json)  |
| Prototypes       | [Document](./files/56/prototypes/document.json)       | [Page](./files/56/prototypes/pages/3E878D5F-B097-4A8C-9AB7-F2ECB5BA8874.json)       | [Meta](./files/56/prototypes/meta.json)       | [User](./files/56/prototypes/user.json)       |
| Shape paths      | [Document](./files/56/shape-paths/document.json)      | [Page](./files/56/shape-paths/pages/3DE941E6-4221-4232-9DC1-0FEA2D1CC76E.json)      | [Meta](./files/56/shape-paths/meta.json)      | [User](./files/56/shape-paths/user.json)      |
| Shapes           | [Document](./files/56/shapes/document.json)           | [Page](./files/56/shapes/pages/291D1A22-E39E-42E5-9359-933935BFD545.json)           | [Meta](./files/56/shapes/meta.json)           | [User](./files/56/shapes/user.json)           |
| Symbol overrides | [Document](./files/56/symbol-overrides/document.json) | [Page](./files/56/symbol-overrides/pages/0982D305-0E02-4C43-A6EA-3AAE18BDB172.json) | [Meta](./files/56/symbol-overrides/meta.json) | [User](./files/56/symbol-overrides/user.json) |
| Symbols          | [Document](./files/56/symbols/document.json)          | [Page](./files/56/symbols/pages/57823E51-CA2F-4D65-8C5A-EB80DFBEDB1A.json)          | [Meta](./files/56/symbols/meta.json)          | [User](./files/56/symbols/user.json)          |
| Text             | [Document](./files/56/text/document.json)             | [Page](./files/56/text/pages/E16DCEB0-E7DA-4F89-81CA-4E4CFCAC8F75.json)             | [Meta](./files/56/text/meta.json)             | [User](./files/56/text/user.json)             |

### Sketch 55.2 (document `v119`)

| Feature          |                                                         |                                                                                       |                                                 |                                                 |
| ---------------- | ------------------------------------------------------- | ------------------------------------------------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- |
| Empty            | [Document](./files/55.2/empty/document.json)            | [Page](./files/55.2/empty/pages/462E6238-04E5-403D-A8F6-544D95F82FCB.json)            | [Meta](./files/55.2/empty/meta.json)            | [User](./files/55.2/empty/user.json)            |
| Groups           | [Document](./files/55.2/groups/document.json)           | [Page](./files/55.2/groups/pages/7F3EED58-6BE4-4D31-A43E-0E666813AFEC.json)           | [Meta](./files/55.2/groups/meta.json)           | [User](./files/55.2/groups/user.json)           |
| Images           | [Document](./files/55.2/images/document.json)           | [Page](./files/55.2/images/pages/DFFECD23-A582-4671-AD51-6E8A37441A4E.json)           | [Meta](./files/55.2/images/meta.json)           | [User](./files/55.2/images/user.json)           |
| Library styles   | [Document](./files/55.2/library-styles/document.json)   | [Page](./files/55.2/library-styles/pages/9B3E5345-A82C-40FA-AA08-5BE8C8E95DAE.json)   | [Meta](./files/55.2/library-styles/meta.json)   | [User](./files/55.2/library-styles/user.json)   |
| Library symbols  | [Document](./files/55.2/library-symbols/document.json)  | [Page](./files/55.2/library-symbols/pages/3924C573-7828-4165-9C8B-95C4E27CC31C.json)  | [Meta](./files/55.2/library-symbols/meta.json)  | [User](./files/55.2/library-symbols/user.json)  |
| Prototypes       | [Document](./files/55.2/prototypes/document.json)       | [Page](./files/55.2/prototypes/pages/5A4E56D9-44AC-40B8-AEF6-E86FF0E8B52B.json)       | [Meta](./files/55.2/prototypes/meta.json)       | [User](./files/55.2/prototypes/user.json)       |
| Shape paths      | [Document](./files/55.2/shape-paths/document.json)      | [Page](./files/55.2/shape-paths/pages/0A4180EC-61D3-4E09-8037-1837DBFB96C7.json)      | [Meta](./files/55.2/shape-paths/meta.json)      | [User](./files/55.2/shape-paths/user.json)      |
| Shapes           | [Document](./files/55.2/shapes/document.json)           | [Page](./files/55.2/shapes/pages/C2442298-D235-4348-93AB-78A03E72B5CD.json)           | [Meta](./files/55.2/shapes/meta.json)           | [User](./files/55.2/shapes/user.json)           |
| Symbol overrides | [Document](./files/55.2/symbol-overrides/document.json) | [Page](./files/55.2/symbol-overrides/pages/9AD6830D-9193-4CD4-BB48-71E1F4430AD2.json) | [Meta](./files/55.2/symbol-overrides/meta.json) | [User](./files/55.2/symbol-overrides/user.json) |
| Symbols          | [Document](./files/55.2/symbols/document.json)          | [Page](./files/55.2/symbols/pages/002D48DE-C55F-4F8C-8812-D189ED2579D8.json)          | [Meta](./files/55.2/symbols/meta.json)          | [User](./files/55.2/symbols/user.json)          |
| Text             | [Document](./files/55.2/text/document.json)             | [Page](./files/55.2/text/pages/571ACF6A-9B1C-49D9-B39A-6AE1D40EF938.json)             | [Meta](./files/55.2/text/meta.json)             | [User](./files/55.2/text/user.json)             |

### Sketch 55.1 (document `v118`)

| Feature          |                                                         |                                                                                       |                                                 |                                                 |
| ---------------- | ------------------------------------------------------- | ------------------------------------------------------------------------------------- | ----------------------------------------------- | ----------------------------------------------- |
| Empty            | [Document](./files/55.1/empty/document.json)            | [Page](./files/55.1/empty/pages/838FC075-E787-404C-BE3A-F9F572905235.json)            | [Meta](./files/55.1/empty/meta.json)            | [User](./files/55.1/empty/user.json)            |
| Groups           | [Document](./files/55.1/groups/document.json)           | [Page](./files/55.1/groups/pages/DC3EA4A4-81B2-4566-B7BE-738AD2E46CDD.json)           | [Meta](./files/55.1/groups/meta.json)           | [User](./files/55.1/groups/user.json)           |
| Images           | [Document](./files/55.1/images/document.json)           | [Page](./files/55.1/images/pages/84EA6DA7-EC56-4034-BBC6-6653F00B9015.json)           | [Meta](./files/55.1/images/meta.json)           | [User](./files/55.1/images/user.json)           |
| Library styles   | [Document](./files/55.1/library-styles/document.json)   | [Page](./files/55.1/library-styles/pages/62C72E39-1992-4A15-B5AE-63564398CF9C.json)   | [Meta](./files/55.1/library-styles/meta.json)   | [User](./files/55.1/library-styles/user.json)   |
| Library symbols  | [Document](./files/55.1/library-symbols/document.json)  | [Page](./files/55.1/library-symbols/pages/CCE1EDAF-8995-490D-B011-D996AF420117.json)  | [Meta](./files/55.1/library-symbols/meta.json)  | [User](./files/55.1/library-symbols/user.json)  |
| Prototypes       | [Document](./files/55.1/prototypes/document.json)       | [Page](./files/55.1/prototypes/pages/1F9C12E8-C269-4573-83EA-597C2092C277.json)       | [Meta](./files/55.1/prototypes/meta.json)       | [User](./files/55.1/prototypes/user.json)       |
| Shape paths      | [Document](./files/55.1/shape-paths/document.json)      | [Page](./files/55.1/shape-paths/pages/5BFC3AA6-F5D9-4FD0-A82E-74559D93F896.json)      | [Meta](./files/55.1/shape-paths/meta.json)      | [User](./files/55.1/shape-paths/user.json)      |
| Shapes           | [Document](./files/55.1/shapes/document.json)           | [Page](./files/55.1/shapes/pages/91028695-2E7F-4C2B-B124-E56257406567.json)           | [Meta](./files/55.1/shapes/meta.json)           | [User](./files/55.1/shapes/user.json)           |
| Symbol overrides | [Document](./files/55.1/symbol-overrides/document.json) | [Page](./files/55.1/symbol-overrides/pages/2C87A6F2-4D14-4976-AF78-D83719143B51.json) | [Meta](./files/55.1/symbol-overrides/meta.json) | [User](./files/55.1/symbol-overrides/user.json) |
| Symbols          | [Document](./files/55.1/symbols/document.json)          | [Page](./files/55.1/symbols/pages/AAFA6543-CC89-42FE-B527-A55AFBEBA3EA.json)          | [Meta](./files/55.1/symbols/meta.json)          | [User](./files/55.1/symbols/user.json)          |
| Text             | [Document](./files/55.1/text/document.json)             | [Page](./files/55.1/text/pages/F668A9E4-2F4F-4177-9368-D5BF93491055.json)             | [Meta](./files/55.1/text/meta.json)             | [User](./files/55.1/text/user.json)             |

### Sketch 55 (document `v118`)

| Feature          |                                                       |                                                                                     |                                               |                                               |
| ---------------- | ----------------------------------------------------- | ----------------------------------------------------------------------------------- | --------------------------------------------- | --------------------------------------------- |
| Empty            | [Document](./files/55/empty/document.json)            | [Page](./files/55/empty/pages/C4D34DD6-C1EE-457E-8896-120526C59310.json)            | [Meta](./files/55/empty/meta.json)            | [User](./files/55/empty/user.json)            |
| Groups           | [Document](./files/55/groups/document.json)           | [Page](./files/55/groups/pages/E4C01AA8-EDD3-4339-A3F5-951707D958AA.json)           | [Meta](./files/55/groups/meta.json)           | [User](./files/55/groups/user.json)           |
| Images           | [Document](./files/55/images/document.json)           | [Page](./files/55/images/pages/BC75AA32-518F-489E-9388-F70C758546F3.json)           | [Meta](./files/55/images/meta.json)           | [User](./files/55/images/user.json)           |
| Library styles   | [Document](./files/55/library-styles/document.json)   | [Page](./files/55/library-styles/pages/4849E1C6-21C5-415B-AE45-A31AEEDD47BC.json)   | [Meta](./files/55/library-styles/meta.json)   | [User](./files/55/library-styles/user.json)   |
| Library symbols  | [Document](./files/55/library-symbols/document.json)  | [Page](./files/55/library-symbols/pages/89A0687B-6B49-4699-9ECB-488BCE2A4066.json)  | [Meta](./files/55/library-symbols/meta.json)  | [User](./files/55/library-symbols/user.json)  |
| Prototypes       | [Document](./files/55/prototypes/document.json)       | [Page](./files/55/prototypes/pages/5394B55B-C6F5-49C6-B384-B336AEB715DD.json)       | [Meta](./files/55/prototypes/meta.json)       | [User](./files/55/prototypes/user.json)       |
| Shape paths      | [Document](./files/55/shape-paths/document.json)      | [Page](./files/55/shape-paths/pages/AB6EBFFB-05F9-4E10-B2F3-8F62317351F0.json)      | [Meta](./files/55/shape-paths/meta.json)      | [User](./files/55/shape-paths/user.json)      |
| Shapes           | [Document](./files/55/shapes/document.json)           | [Page](./files/55/shapes/pages/E8CF0BBE-7488-45BB-B458-65AD65749F2E.json)           | [Meta](./files/55/shapes/meta.json)           | [User](./files/55/shapes/user.json)           |
| Symbol overrides | [Document](./files/55/symbol-overrides/document.json) | [Page](./files/55/symbol-overrides/pages/5D034CE6-E63C-4244-86D9-721E9FE62C06.json) | [Meta](./files/55/symbol-overrides/meta.json) | [User](./files/55/symbol-overrides/user.json) |
| Symbols          | [Document](./files/55/symbols/document.json)          | [Page](./files/55/symbols/pages/0347FF79-264E-45FC-B815-01BB8FABE578.json)          | [Meta](./files/55/symbols/meta.json)          | [User](./files/55/symbols/user.json)          |
| Text             | [Document](./files/55/text/document.json)             | [Page](./files/55/text/pages/CF18D727-5650-4FA0-AA00-BD40AA412CF0.json)             | [Meta](./files/55/text/meta.json)             | [User](./files/55/text/user.json)             |
