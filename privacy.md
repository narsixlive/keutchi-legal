# Politique de confidentialité — Keutchi

**Dernière mise à jour : 2026-06-01**

## 1. Responsable du traitement

L'application mobile Keutchi (« l'Application ») est éditée par :

- **Nom / Raison sociale :** Matheo Congé
- **Statut :** Particulier
- **Adresse :** *Coordonnées disponibles auprès de l'hébergeur sur réquisition judiciaire, conformément à l'article 1-1 de la LCEN.*
- **Email contact :** contact@keutchi.app
- **Directeur de la publication :** Matheo Congé

L'éditeur est responsable du traitement des données personnelles collectées via l'Application au sens de l'article 4(7) du RGPD.

## 2. Délégué à la protection des données

L'Application n'a pas l'obligation légale de désigner un DPO. Pour toute question relative à vos données personnelles, contactez : **contact@keutchi.app**.

## 3. Données collectées

### 3.1 Données fournies par l'utilisateur

| Donnée | Origine | Obligatoire |
|---|---|---|
| Adresse email | Création de compte | ✅ |
| Pseudonyme (handle) | Choix utilisateur après inscription | ✅ |
| Nom affiché, avatar | Optionnel (profil) | ❌ |
| Favoris / events intéressés | Action utilisateur | ❌ |

### 3.2 Données collectées automatiquement

| Donnée | Finalité | Conservation |
|---|---|---|
| Adresse IP **hachée** (SHA-256, 16 caractères, sel rotatif) | Limitation du débit du redirecteur de billetterie (anti-abus) | 1 heure max |
| Compteur de clics sur les events (agrégé par jour) | Mesure d'audience first-party (cf. §5 — exempte de consentement CNIL) | 24 mois |
| Rapports de crash via Sentry | Stabilité de l'Application | 90 jours |
| Métriques de performance via Sentry (10% des transactions) | Optimisation | 90 jours |

Les informations personnelles identifiantes (email, IP en clair, identifiant utilisateur) sont **systématiquement supprimées** par notre code avant tout envoi à Sentry (`beforeSend` hook).

### 3.3 Données **non** collectées

- ❌ Localisation GPS précise ou approximative
- ❌ Carnet de contacts
- ❌ Identifiants publicitaires (IDFA / GAID)
- ❌ Données de tracking cross-app
- ❌ Cookies tiers
- ❌ Données comportementales pour publicité

## 4. Finalités et bases légales

| Finalité | Données utilisées | Base légale RGPD |
|---|---|---|
| Création et gestion de votre compte | Email, handle | Art. 6(1)(b) — Exécution du contrat |
| Affichage des concerts et événements | Aucune donnée personnelle requise | Art. 6(1)(f) — Intérêt légitime |
| Sauvegarde de vos favoris | Identifiant utilisateur, event_id | Art. 6(1)(b) — Exécution du contrat |
| Redirection vers les billetteries | event_id, IP hachée | Art. 6(1)(f) — Intérêt légitime (sécurisation) |
| Mesure d'audience first-party (compteur de clics) | event_id agrégé | Art. 6(1)(f) — Intérêt légitime + CNIL fiche n°16 (exempt de consentement) |
| Diagnostic et correction des bugs | Crash logs, perf | Art. 6(1)(f) — Intérêt légitime |

**Mesure d'audience first-party** : Conformément à la fiche n°16 de la CNIL ("Use analytics on your websites and applications"), notre compteur de clics est **exempt de consentement** car il remplit cumulativement les conditions : (1) finalité strictement limitée à la mesure d'audience, (2) données anonymisées (IP hachée, agrégation par jour), (3) aucun croisement avec d'autres traitements, (4) aucune transmission à des tiers, (5) aucun suivi cross-app.

## 5. Destinataires et sous-traitants

Vos données sont accessibles uniquement à l'éditeur. Les sous-traitants techniques suivants sont impliqués :

| Sous-traitant | Rôle | Localisation des données |
|---|---|---|
| **Supabase Inc.** | Hébergement de la base de données, authentification | Frankfurt (DE) ou Dublin (IE), UE |
| **Sentry GmbH** | Crash reporting et monitoring de performance | Allemagne, UE |
| **Google LLC** | Distribution de l'Application (Google Play) + authentification OAuth | États-Unis |
| **Intuition Machines, Inc. (hCaptcha)** | Protection anti-bot du formulaire de connexion | États-Unis |
| **Cloudflare** | CDN images (le cas échéant) | UE |

Aucune donnée personnelle n'est vendue ni transmise à des fins publicitaires.

## 6. Transferts hors UE

Les données de compte et d'utilisation sont hébergées dans l'Union européenne. Le sous-traitant Google peut transférer certaines métadonnées (téléchargements, identifiants de compte store) hors UE dans le cadre de la distribution de l'Application — ces traitements sont régis par ses propres politiques de confidentialité.

## 7. Durée de conservation

| Donnée | Durée |
|---|---|
| Compte utilisateur (email, handle, profil) | Jusqu'à suppression du compte par l'utilisateur, ou 24 mois d'inactivité |
| Favoris et events intéressés | Idem compte utilisateur |
| Crash logs | 90 jours |
| Compteur de clics agrégé | 24 mois |
| IP hachée (rate-limiting) | 1 heure max |
| Sauvegardes hebdomadaires de la base | 90 jours |

## 8. Vos droits

Conformément aux articles 15 à 22 du RGPD, vous disposez des droits suivants :

- **Droit d'accès** : obtenir une copie de vos données
- **Droit de rectification** : corriger vos données inexactes
- **Droit à l'effacement** ("droit à l'oubli") : supprimer votre compte et toutes vos données associées
- **Droit à la limitation** du traitement
- **Droit à la portabilité** : récupérer vos données dans un format structuré
- **Droit d'opposition** au traitement basé sur l'intérêt légitime
- **Droit de retirer votre consentement** à tout moment

**Suppression du compte** : disponible directement dans l'Application via `Compte → Supprimer mon compte`. La suppression est immédiate et définitive (cascade sur toutes vos données associées).

**Pour exercer vos autres droits** : écrivez à **contact@keutchi.app**. Une réponse vous sera apportée sous **30 jours** maximum (art. 12(3) RGPD).

**Recours CNIL** : si vous estimez que vos droits ne sont pas respectés, vous pouvez introduire une réclamation auprès de la CNIL (3 Place de Fontenoy, 75007 Paris, [www.cnil.fr](https://www.cnil.fr)).

## 9. Sécurité

Mesures techniques mises en œuvre :

- Chiffrement TLS 1.3 de toutes les communications client ↔ serveur
- Authentification par JWT signé (Supabase Auth)
- Politiques Row-Level Security (RLS) "default-deny" sur l'ensemble des tables sensibles
- Hachage SHA-256 systématique des adresses IP avant tout stockage
- Anonymisation des rapports d'erreur (suppression PII avant envoi)
- Sauvegardes chiffrées hebdomadaires
- Aucun mot de passe stocké (authentification par lien magique ou OAuth)

## 10. Mineurs

L'Application n'est pas spécifiquement destinée aux mineurs de moins de 15 ans (seuil RGPD France). En cas d'inscription d'un mineur, le consentement des titulaires de l'autorité parentale est requis. Pour signaler l'inscription d'un mineur sans autorisation : **contact@keutchi.app**.

## 11. Modifications

L'éditeur se réserve le droit de modifier la présente politique de confidentialité. Toute modification substantielle sera notifiée via l'Application avec un préavis de **30 jours** avant entrée en vigueur. La poursuite de l'utilisation après ce délai vaut acceptation.

## 12. Contact

Pour toute question relative à vos données personnelles ou à cette politique : **contact@keutchi.app**.
