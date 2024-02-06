# Commit Guidelines:

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED",  "MAY", and "OPTIONAL" in this document are to be interpreted as described in [RFC 2119](https://tools.ietf.org/html/rfc2119).

Exceptions **SHOULD** be made by contacting the administration team.

- The commit's message **MUST** have its content clear to anyone that wants to know what the commit is about. There is absolutely no need for the commit message to contain Linux Foundation like documentation, however something that an average newbie developer would understand is required. Extra documentation/explanation **MUST** be there if the commit's content is huge, and also will always be welcome.

- The commit's message **MUST** have an indicator of where the commit introduces changes, following the standard: "<path/repository name reference>: <Commit title that **MUST** be a basic explanation for its content>".

- The commit **MUST** be necessary for a device to build, boot, to have a device's function(s) working properly (e.g. Fingerprint On Display) or to enhance the working of already working features on the ROM side.

- The commit **MUST** have proper authorship.

- If a commit is for the ROM side, the same **MUST** be pushed to [Gerrit](https://gerrit.pixelexperience.org).

- The commit's content **MUST** be as minimal and polished as possible.

- The commit **MUST** be in accordance with the items, if applicable, stated at our [Maintainers Code of Conduct](https://github.com/PixelExperience/docs/blob/master/maintainers_code_of_conduct.md).

- For revert commits, the same **SHOULD** contain reason for revert point - if possible at all. As stated previously, any extra bit of documentation in the commit's message is welcome.

