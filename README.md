# UnityPackageTemplate
a template sample for create a custom unity package

## [Creating custom packages](https://docs.unity3d.com/Manual/CustomPackages.html)

### [Package layout](https://docs.unity3d.com/Manual/cus-layout.html)

    <root>
    ├── package.json
    ├── README.md
    ├── CHANGELOG.md
    ├── LICENSE.md
    ├── Third Party Notices.md
    ├── Editor
    │   ├── [company-name].[package-name].Editor.asmdef
    │   └── EditorExample.cs
    ├── Runtime
    │   ├── [company-name].[package-name].asmdef
    │   └── RuntimeExample.cs
    ├── Tests
    │   ├── Editor
    │   │   ├── [company-name].[package-name].Editor.Tests.asmdef
    │   │   └── EditorExampleTest.cs
    │   └── Runtime
    │        ├── [company-name].[package-name].Tests.asmdef
    │        └── RuntimeExampleTest.cs
    ├── Samples~
    │        ├── SampleFolder1
    │        ├── SampleFolder2
    │        └── ...
    └── Documentation~
        └── [package-name].md



### [Package manifest](https://docs.unity3d.com/Manual/upm-manifestPkg.html)


```json
{
  "name": "com.[company-name].[package-name]",
  "version": "1.2.3",
  "displayName": "Package Example",
  "description": "This is an example package",
  "unity": "2019.1",
  "unityRelease": "0b5",
  "documentationUrl": "https://example.com/",
  "changelogUrl": "https://example.com/changelog.html",
  "licensesUrl": "https://example.com/licensing.html",
  "dependencies": {
    "com.[company-name].some-package": "1.0.0",
    "com.[company-name].other-package": "2.0.0"
 },
 "keywords": [
    "keyword1",
    "keyword2",
    "keyword3"
  ],
  "author": {
    "name": "Unity",
    "email": "unity@example.com",
    "url": "https://www.unity3d.com"
  }
}

```

## Share Package

### [Scoped Registries](https://docs.unity3d.com/2020.3/Documentation/Manual/upm-scoped.html)