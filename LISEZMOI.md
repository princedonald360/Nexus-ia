# NEXUS AI : installation depuis votre téléphone (sans ordinateur)

## Les 5 fichiers
`index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`

## Applications et comptes gratuits nécessaires
| Besoin | Outil gratuit | Remarque |
|---|---|---|
| Navigateur | **Chrome** (Android) ou **Safari** (iPhone) | Déjà installé. Sert à héberger, installer et utiliser l'app. |
| Hébergement HTTPS | Compte **GitHub** + **GitHub Pages** | Tout se fait depuis le site github.com dans le navigateur. L'application GitHub est facultative. |
| IA (cerveau de l'app) | Clé API gratuite **Google Gemini** : https://aistudio.google.com/apikey | Alternatives : **Groq** (console.groq.com/keys) ou **OpenRouter** (openrouter.ai/keys). La disponibilité du gratuit dépend de votre pays : à vérifier à la création de la clé. |
| Modifier le code (facultatif) | **Acode** (Android, éditeur gratuit) | Inutile si vous me demandez les modifications. |

Aucun logiciel à compiler : l'application est un simple site web installable (PWA).

## Étapes
1. **Récupérer les 5 fichiers** sur le téléphone (téléchargements depuis Claude).
2. Créer un compte sur **github.com**, puis **New repository** : nom `nexus-ai`, **Public**, cocher « Add a README ».
3. Dans le dépôt : **Add file → Upload files**, sélectionner les 5 fichiers, puis **Commit changes**.
4. **Settings → Pages** : *Source* = « Deploy from a branch », branche `main`, dossier `/ (root)`, **Save**.
5. Attendre 1 à 2 minutes. L'adresse est : `https://VOTRE-PSEUDO.github.io/nexus-ai/`
6. Ouvrir cette adresse dans Chrome/Safari.
7. **Installer** : Chrome ⋮ → « Installer l'application » (ou « Ajouter à l'écran d'accueil »). Safari : Partager → « Sur l'écran d'accueil ».
8. Dans l'app : ⚙ **Paramètres → Intelligence artificielle** : choisir Gemini, coller la clé, **Enregistrer**, puis **Tester la connexion**.

Le dépôt est public, mais il ne contient **aucune clé ni donnée personnelle** : vos données et votre clé restent dans le navigateur de votre téléphone.

## État réel des fonctions (V1 téléphone seul)
**Opérationnelles** : chat avec historique, projets, tâches (aujourd'hui / à venir / en retard), mémoire contrôlable, import PDF/DOCX/XLSX/CSV/TXT/images, résumé, analyse, recherche de passage, comparaison, export DOCX / PDF / MD / TXT, workflows séquentiels avec validation et journal, recherche web sourcée (Gemini), code de verrouillage, sauvegarde JSON, thème sombre, installation PWA.

**Limites assumées** : pas de compte multi-appareils ni synchronisation (données locales à ce téléphone, pensez à exporter une sauvegarde) ; pas d'OCR pour les PDF scannés ; pas de rappels/notifications ; pas d'envoi d'email ni d'agenda ; pas de serveur MCP ChatGPT ; le code de verrouillage ne chiffre pas les données ; le PDF passe par la fenêtre d'impression (« Enregistrer au format PDF »). Les quotas gratuits des fournisseurs IA limitent le nombre de requêtes (compteur et plafond quotidien dans Paramètres).

Ces limites viennent de l'absence de serveur : elles correspondent aux fonctions « à connecter » du cahier des charges.

## Mettre à jour l'app
Remplacer un fichier sur GitHub (Add file → Upload files, même nom). Fermer puis rouvrir l'app deux fois pour recharger la nouvelle version.
