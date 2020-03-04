([Français](#exemple-d'installation-WiX-pour-les-fichiers-statiques))

# Example WiX Installer for Static Files
A sample of installing a sample legacy DLL that just need to get to the right place and get registered.

> **Note:** The core components / static files have been removed from the project as they are not the focus of the project. 
> 
> Files removed: 
> - `\TCMailer_TC3oE\TC Mailer 3.0.dll`
> - `\TCMailer_TC3oE\TCMailer.ini`

This is an installer that has no UI or parameters. 

It is just get a legacy library installed in the GAC and a few registry entries.

## Required Components / Reading
- [WiX Download Page](https://wixtoolset.org/releases/)
  - WiX Toolset installed somewhere
  - WiX Visual Studio Extension (to handle .wixproj files and wrap utility calls)
  - [WiX Toolset Reference](https://wixtoolset.org/documentation/manual/v3/)
- Visual Studio (Community Edition used in this project)

## Instructions
To run *as-is*, replace the two removed files with other files or empty ones to be able 'build' in Visual Studio.

The rest of the tweaking and customization is all contained in the `\TCMailer_TC3oE\Product.wxs` file.

## Useful Links 
- [Online GUID Generator](https://www.guidgenerator.com/online-guid-generator.aspx)
- [dnSpy .NET DLL Decompiler](https://github.com/0xd4d/dnSpy)
- [A pretty good sample WXS](https://helgeklein.com/blog/2014/09/real-world-example-wix-msi-application-installer/#product-wxs)

---

# Exemple d'installation WiX pour les fichiers statiques
Un exemple d'installation d'un exemple de DLL héritée qui doit simplement se rendre au bon endroit et être enregistré.

> ** Remarque: ** Les composants principaux / fichiers statiques ont été supprimés du projet car ils ne sont pas au centre du projet.
>
> Fichiers supprimés:
> - `\TCMailer_TC3oE\TC Mailer 3.0.dll`
> - `\TCMailer_TC3oE\TCMailer.ini`

Il s'agit d'un programme d'installation qui n'a pas d'interface utilisateur ou de paramètres.

Il suffit d'obtenir une bibliothèque héritée installée dans le GAC et quelques entrées de registre.

## Composants requis / lecture
- [Page de téléchargement WiX](https://wixtoolset.org/releases/)
  - WiX Toolset installé quelque part
  - Extension WiX Visual Studio (pour gérer les fichiers .wixproj et encapsuler les appels de l'utilitaire)
  - [Référence de l'ensemble d'outils WiX](https://wixtoolset.org/documentation/manual/v3/)
- Visual Studio (Community Edition utilisé dans ce projet)

## Instructions
Pour exécuter *tel quel*, remplacez les deux fichiers supprimés par d'autres fichiers ou des fichiers vides pour pouvoir «créer» dans Visual Studio.

Le reste des ajustements et de la personnalisation sont tous contenus dans le fichier `\TCMailer_TC3oE\Product.wxs`.

## Liens utiles
- [Générateur de GUID en ligne](https://www.guidgenerator.com/online-guid-generator.aspx)
- [dnSpy .NET DLL décompilateur](https://github.com/0xd4d/dnSpy)
- [Un très bon exemple de WXS](https://helgeklein.com/blog/2014/09/real-world-example-wix-msi-application-installer/#product-wxs)
