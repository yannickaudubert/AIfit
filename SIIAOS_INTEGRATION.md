# Intégration au puzzle SIIAOS

```yaml
siiaos_puzzle_version: "2026-09-25"
integration_status: "CANDIDATE"
truth_status: "NOT_PROVEN_AS_SIIAOS_COMPONENT"
authority: "none"
canonical_reference: "yannickaudubert/twinSIIAOS/docs/SIIAOS_PUZZLE.md"
```

## Rôle

Candidat Capability provider pour l'adéquation modèles/hardware et l'aide au routage local. Le dépôt dérive de llmfit et n'est pas admis automatiquement au SIIAOS.

## Ce que cette brique implique

- Ses scores sont des aides à la décision, pas des autorisations ni des benchmarks SIIAOS prouvés.
- Une recommandation de modèle doit être confrontée aux besoins, données, licences, qualité observée et runtime réel.
- Aucune installation ou activation ne découle automatiquement d'un résultat llmfit/AIfit.

## Capabilities fournies

- hardware detection
- model fit estimation
- model shortlist/recommendations
- optional local REST capability

## Capabilities consommées

- ObservedState hardware
- model metadata
- NeedSpec/use-case
- runtime policy

## Evidence minimale avant promotion

- reproducible hardware probe
- fit calculation tests
- runtime benchmark before admission
- license/source review

## Non-rôles

- Model Gateway
- autorité de routage
- benchmark métier suffisant
- preuve d'installation

## Invariants

- `PROPOSÉ != CODÉ != TESTÉ != DÉPLOYÉ != OBSERVÉ != PROUVÉ`.
- `DesiredState != ObservedState`.
- Trouvé ou présent dans GitHub ne signifie pas intégré, installé, sûr ou opérationnel.
- Une capacité ne crée pas une autorité.
- Une donnée confidentielle ne devient pas transverse par apprentissage implicite.
- Une admission future doit préciser permissions, données, interfaces, Evidence, fallback et retrait.

## Référence

Le puzzle complet et le contrat documentaire commun sont maintenus dans `twinSIIAOS/docs/`. Cette fiche sert uniquement à classifier ce dépôt et à empêcher une admission implicite.
