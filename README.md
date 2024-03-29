# WGSExtract-Historical

Former wgsextract.github.io entry page:
# WGS Extract v2b (last)
a desktop tool for verifying, analyzing and manipulating your **DTC 30x [WGS](https://h600.org/wiki/WGS) test** results

__Current release__ is Beta v2b (18 Feb 2020 through to 15 Jun 2021):
* **WGS Extract** [Manual (Google Doc)](http://bit.ly/36Jdpnq)  
* **WGS Extract** [Download Release (5 GB)](http://bit.ly/3afRl6O) (`see below for alternative`)
```
SHA256: 41D68ED9ABEAAD0AA6BB68F3043294DC02F5DD17E28F86BB776C56704148F76C
MD5: 690C3C6D5CFBF745114D1690C4C00065
```
[More information on hashes used to verify the download release is available](https://www.howtogeek.com/67241/htg-explains-what-are-md5-sha-1-hashes-and-how-do-i-check-them/)

Finding the initial download too large? See the **Alternate** at the end here for a patched download that can be performed in stages. 

Still waiting for your WGS test results?  Want to get started today?  See the [International Genome Sample Resource (1K Genome archive)](https://www.internationalgenome.org/data) for BAM files that you can download and play with to learn the tool while waiting for your results.

**`Note`**: MacOS 11 on M1 systems is having [issues with the MacPorts tools](https://trac.macports.org/wiki/BigSurProblems). We are waiting for Apple and Macports to find a solution.  Also, since switching to our Google Drive delivery cloud, it seems Safari may be needed to download in MacOS on M1. See our special [MacOSX Release Patch](https://github.com/WGSExtract/WGSExtract-Dev/blob/master/Docs/Betav2b_MacOSX_patch.md) for further notes.

**`IMPORTANT`**: [MacOSX Release Patch](https://github.com/WGSExtract/WGSExtract-Dev/blob/master/Docs/Betav2b_MacOSX_patch.md) is available for Version Beta v2b.  Fixes the install and start scripts of the program. Adds an Unintall as well. (v1 on 25 April 2020, v3 on 20 Jun 2020, v5 on 31 Oct 2020)

**`Note`**: [Français Language Patch](https://github.com/WGSExtract/WGSExtract-Dev/blob/master/Docs/Betav2b_Francais_Patch.md) is available for Version Beta v2b.  Adds Français language support to the existing English and Deutsch language support. (1 May 2020)

**`Note`**: If working with a Nebula Genomics CRAM file, please [check the CRAM to BAM conversion document](https://bit.ly/31TeqYH). The next release will handle CRAMs and BAMs interchangeably.

This tool is geared toward the needs of [genetic genealogy](https://h600.org/wiki/Genetic+Genealogy) but may be helpful for those looking into health-releated uses of WGS tests. The **sub-$500, Direct-to-Consumer (DTC), 30x Whole Genome Sequence (WGS) tests** are delivered with basic data files and reports. This tool serves to bridge the gap between the [WGS files](https://h600.org/wiki/Sequencing+File+Formats) delivered and the present day [genetic genealogy community tools](https://h600.org/wiki/Third+Party+Analysis+Tools). Many health analysis sites accept the microarray and VCF files generated here as well.

This tool is designed to be a simple, push-button manipulation of [WGS files](https://h600.org/wiki/Sequencing+File+Formats) from any source. It hides the scripting of complex bioinformatic tools and automatically determines needed parameters and variances for the data supplied it.  For more control over your pipeline, either learn to use the underlying tools directly in a command shell or seek a Galaxy server (such as [UseGalaxy](https://usegalaxy.org/)).

The tool has the potential to be a simple install in a BioConda environment as it is primarily a Python package. But as a majority of the users are on Microsoft Windows 10 systems, and Bioconda nor the underlying bioinformatic tools are not available there, we currently deliver the tool as a more complex, "deliver everything" approach. This may change going forward after we find a Win10 package manager to supply the bioinformatic tool ports we develop here. We do fully test and use the Linux and Apple MaxOS versions. This is the only source of the bioinformatic tools on a Win10 system (that we are aware of).

We use the Facebook group [Dante Labs and Nebula Genomics Customers](https://www.facebook.com/groups/373644229897409/) for discussions on how to make use of your **sub-$500, DTC 30x WGS test** results. Bugs, use cases and announcements about this tool happen there.  As part of that Facebook groups' Files section, you will find a number of useful companion documents and tool references.  In particular, start with [Bioinformatics for Newbies](http://bit.ly/38jnxnK).

User issues, if not brought up in the [Facebook group](https://www.facebook.com/groups/373644229897409/), should be raised in the [user issues section of this site](https://github.com/WGSExtract/WGSExtract.github.io/issues). This issues section is the preferred location so code bugs, use limitations and suggested improvements can be tracked within the development project.

The tool acronym is **WGSE** and is pronounced as "wig-see". We encourage that use in English language conversation.

Further documentation (beyond the manual link above) is available in our [WGS Extract Developer's Documentation Repository](https://github.com/WGSExtract/WGSExtract-Dev/tree/master/Docs).

Developer's should visit the main GitHub [WGS Extract Developers Code Repository](https://github.com/WGSExtract/WGSExtract-Dev/).  Development issues, code bugs and limitations should be [raised in the development issues section](https://github.com/WGSExtract/WGSExtract-Dev/issues) so they are tracked till resolved in a release.

The original, first year, [historical release is documented here](https://github.com/WGSExtract/WGSExtract-Historical).

This page is located at https://WGSExtract.github.io/ and serves as the new WWW home for the tool. As the need develops, we will create our own Facebook Group for users to raise issues outside of the [User Issues Section](https://github.com/WGSExtract/WGSExtract.github.io/issues) already mentioned.

**UPDATE** `One Year Later (Feb 2021)`:
The BetaV2b release is simple.  The 4.5 GB zip archive consists of 4.2 GB of Human Genome Reference Models that are sometimes needed. But it is this large size that gives some issues with downloading.  Therefore, we have created three separate .zip archives to aid the process.

__WGS Extract release__ of Beta v2b (18 Feb 2020) broken up into separate ZIP archives (including all patches already applied):
* [Main Program Release and Support Files](http://bit.ly/3usF3RN) (170 MB of Python and BASH scripts; reference tables, JAR file)
* [Reference Genomes](http://bit.ly/2ZLD3pB) (~4.5 GB compressed; goes in your main installation folder) (needed only if you find a command fails)
* [Win10Execs](http://bit.ly/3bEyTFu) (~80 MB compressed; goes in your programs folder of your main installation) (Only for Microsoft Win10 users)

We are working to make all **Reference Genome** files downloaded on demand in future releases. You can run some features of the tool without the Reference Genomes available. So consider downloading and installing the **Main Program Release** and later adding the **Reference Genomes**. The Win10 tool ports are only needed for Win10 users. In fact, if we even make our own binary templates downloaded as needed, the program drops to under 10 MB downloaded and installed! Clearly a much better solution going forward.

# WGS Extract pre-final v2b
Documenting the initial, first two years WGS Extract Beta releases by Marko from May 2019 through May 2021 and made available (then) at http://37.187.22.93/wgsextract/WGSExtractBeta.zip.

This section is to hold the python source code of the releases and any notes on Marko's first year of releases and support. Manuals and patch mods were by Randy starting 5 months in.

Note that the release ZIP archives included the Reference Genomes and similar large files that exceed limits set by GITHub for storing here.  So you will have to get the complete package .zip release elsewhere. This is just the Python source and related, smaller files that Marko distributed; here for historical reasons.

Marko never checked in the modifications required to create the CygWin WIn10 port of samtools, bcftools, etc; as well as the Python port with its pre-installed libraries. This was all hand developed and the result simply supplied as part of the release in Win10 executable form.  It is not recreatable by anything in this repository.

This work has all been replaced with the new release developed over the last year which is supported and distributed in the main [WGS Extract repository](https://github.com/WGSExtract/WGSExtract "WGS Extract") located here at GitHub also.

We archive the version information for this first release here for historical reasons:

| Version | Dates | Manual | (Archived) Release | Notes|
|:--- | :---:| --- | ---| ---|
| Beta v0|7 May 2019 | - | - |[Initial Release, Win10 Only](https://www.facebook.com/groups/373644229897409/permalink/384165192178646/)
| Beta v1|20 Jun 2019 | - | - |[Update with Autosomal now complete](https://www.facebook.com/photo.php?fbid=2765845590155551&set=p.2765845590155551&type=1&theater)
| Beta v1b| 3 Nov 2019 | - | - |Update to support Autosomal from HG38
| Beta v1c| 24 Nov 2019 |[Manual Beta v1 (Nov 2019)](https://docs.google.com/document/d/1zM-tGKsr-UOMyn1PT4fdy_aEJCy4Wz_q4k-Js3fSpB0/edit?usp=sharing "Manual Beta V1")|[Release Beta v1c (18 Nov 2019) (2 GB)](https://drive.google.com/file/d/1yL7fsk5q8aZzBh6HdWaFTmj_2Dbm50ML/view?usp=sharing) |Added MacOS Support
| Beta v2|29 Dec 2019| - | - |Added Linux Support, Haplogroup tools
| Beta v2b|18 Feb 2020|[Manual Beta v2b (Apr 2020)](https://docs.google.com/document/d/1TqRF_CZMs4QOEuVlrhLkzL-uc-dvHAO92O-S7tc7FhY/edit?usp=drivesdk "Manual Beta v2") | [Release Beta v2b (18 Feb 2020) (5 GB)](http://37.187.22.93/wgsextract/WGSExtractBeta.zip "Release Beta v2b")|[Added Unmapped Read Extraction](https://www.facebook.com/groups/373644229897409/permalink/556793721582458/)

