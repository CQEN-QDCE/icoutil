<!-- ENTETE -->
[![img](https://img.shields.io/badge/Cycle%20de%20Vie-Phase%20D%C3%A9couverte-339999)](https://www.quebec.ca/gouv/politiques-orientations/vitrine-numeriqc/accompagnement-des-organismes-publics/demarche-conception-services-numeriques)
[![License](https://img.shields.io/badge/Licence-Apache--2.0-blue)](LICENSE)

---

<div>
    <a target="_blank" href="https://www.quebec.ca/gouvernement/ministere/cybersecurite-numerique">
      <img src="https://github.com/CQEN-QDCE/.github/blob/main/images/mcn.png" alt="Logo du Ministère de la cybersécurité et du numérique" />
    </a>
</div>
<!-- FIN ENTETE -->

# TL;DR

Use this shell script on macOS to generate all the icon size combinations you need to publish your app to the iTunes and Google Play stores.

## How To

Run `mkicons.sh` to display usage instructions:

```shell
VERSION: 1.0.0
USAGE:
    ./mkicons.sh file destination

DESCRIPTION:
    Generate a complete set of iOS application icons.

    file - The source png image. Preferably above 1024x1024
    destination - The destination path where the icons are output to.

    This script is depend on sips, a small command line utility available on
    macOS.
AUTHOR:
    Jason <jason.leach@fullboar.ca>

LICENSE:
    Apache 2.0

EXAMPLE:
    ./mkicons.sh 1024.png ~/out
```

## How it Works

This script uses `sips`, a built in image process utility on macOS to resize the input image to all the options you need. See the code for exact params.
