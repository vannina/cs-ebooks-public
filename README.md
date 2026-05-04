# Corsica Studio · Ebooks publics

> Hébergement public des 7 ebooks gratuits Corsica Studio.
> Repo public dédié pour fournir des URLs CDN permanentes aux emails de livraison J0.
> Source de vérité PDFs : repo privé `vannina/CS-framer-website` dossier `ebooks/01-pdfs/`.

---

## 7 ebooks disponibles

| Slug | Persona cible | Téléchargement direct |
|---|---|---|
| Découverte | Dirigeant PME | [ebook-1-decouverte.pdf](https://github.com/vannina/cs-ebooks-public/releases/download/v3.0/ebook-1-decouverte.pdf) |
| Prompts | Praticien IA | [ebook-2-prompts.pdf](https://github.com/vannina/cs-ebooks-public/releases/download/v3.0/ebook-2-prompts.pdf) |
| Automatisation | Responsable ops | [ebook-3-automatisation.pdf](https://github.com/vannina/cs-ebooks-public/releases/download/v3.0/ebook-3-automatisation.pdf) |
| BTP | Artisan BTP | [ebook-vertical-btp.pdf](https://github.com/vannina/cs-ebooks-public/releases/download/v3.0/ebook-vertical-btp.pdf) |
| Hôtellerie | Hôtelier indépendant | [ebook-vertical-hotelier.pdf](https://github.com/vannina/cs-ebooks-public/releases/download/v3.0/ebook-vertical-hotelier.pdf) |
| Libéral | Cabinet libéral | [ebook-vertical-liberal.pdf](https://github.com/vannina/cs-ebooks-public/releases/download/v3.0/ebook-vertical-liberal.pdf) |
| Immobilier | Agent immobilier | [ebook-vertical-immobilier.pdf](https://github.com/vannina/cs-ebooks-public/releases/download/v3.0/ebook-vertical-immobilier.pdf) |

---

## Mise à jour des PDFs

Pour publier une nouvelle version :

```bash
cp /Users/vannina/CS-framer-website/ebooks/01-pdfs/*.pdf .
gh release upload v3.0 *.pdf --clobber
```

Les URLs restent identiques, le contenu est mis à jour.

---

## Infrastructure

- **Repo public** : `vannina/cs-ebooks-public` (ce repo)
- **Repo privé source** : `vannina/CS-framer-website` (code Framer + spec ebooks)
- **CDN** : GitHub Releases (Microsoft Azure)
- **Branchement n8n** : workflow `WF-EB-01_Capture_Livraison_Ebook` node Switch → 7 sorties pdfUrl

---

## Contact

- Site : [corsica-studio.com](https://corsica-studio.com)
- Email : contact@corsica-studio.com
- Vannina Michelosi · Ajaccio · Corse
